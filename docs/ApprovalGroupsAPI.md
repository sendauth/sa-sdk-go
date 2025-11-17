# \ApprovalGroupsAPI

All URIs are relative to *https://api.sendauth.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddUserToAuthGroup**](ApprovalGroupsAPI.md#AddUserToAuthGroup) | **Post** /api/v1/approval-groups/{id}/users/{userID} | Add user to approval group
[**CreateAuthGroup**](ApprovalGroupsAPI.md#CreateAuthGroup) | **Post** /api/v1/approval-groups | Create approval group
[**DeleteAuthGroup**](ApprovalGroupsAPI.md#DeleteAuthGroup) | **Delete** /api/v1/approval-groups/{id} | Delete approval group
[**GetAuthGroup**](ApprovalGroupsAPI.md#GetAuthGroup) | **Get** /api/v1/approval-groups/{id} | Get approval group
[**ListAuthGroups**](ApprovalGroupsAPI.md#ListAuthGroups) | **Get** /api/v1/approval-groups | List approval groups
[**RemoveUserFromAuthGroup**](ApprovalGroupsAPI.md#RemoveUserFromAuthGroup) | **Delete** /api/v1/approval-groups/{id}/users/{userID} | Remove user from approval group
[**SetAuthGroupTags**](ApprovalGroupsAPI.md#SetAuthGroupTags) | **Put** /api/v1/approval-groups/{id}/tags | Set approval group tags
[**UpdateAuthGroup**](ApprovalGroupsAPI.md#UpdateAuthGroup) | **Put** /api/v1/approval-groups/{id} | Update approval group



## AddUserToAuthGroup

> AddUserToAuthGroup(ctx, id, userID).Execute()

Add user to approval group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Approval group ID
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | User ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ApprovalGroupsAPI.AddUserToAuthGroup(context.Background(), id, userID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApprovalGroupsAPI.AddUserToAuthGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Approval group ID | 
**userID** | **string** | User ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddUserToAuthGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateAuthGroup

> AuthGroup CreateAuthGroup(ctx).AuthGroup(authGroup).Execute()

Create approval group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go/sa-sdk-go"
)

func main() {
	authGroup := *openapiclient.NewAuthGroup("Name_example", "Threshold_example") // AuthGroup | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApprovalGroupsAPI.CreateAuthGroup(context.Background()).AuthGroup(authGroup).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApprovalGroupsAPI.CreateAuthGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAuthGroup`: AuthGroup
	fmt.Fprintf(os.Stdout, "Response from `ApprovalGroupsAPI.CreateAuthGroup`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAuthGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authGroup** | [**AuthGroup**](AuthGroup.md) |  | 

### Return type

[**AuthGroup**](AuthGroup.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteAuthGroup

> DeleteAuthGroup(ctx, id).Execute()

Delete approval group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Approval group ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ApprovalGroupsAPI.DeleteAuthGroup(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApprovalGroupsAPI.DeleteAuthGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Approval group ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAuthGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAuthGroup

> AuthGroup GetAuthGroup(ctx, id).Execute()

Get approval group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Approval group ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApprovalGroupsAPI.GetAuthGroup(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApprovalGroupsAPI.GetAuthGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAuthGroup`: AuthGroup
	fmt.Fprintf(os.Stdout, "Response from `ApprovalGroupsAPI.GetAuthGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Approval group ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAuthGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AuthGroup**](AuthGroup.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAuthGroups

> []AuthGroup ListAuthGroups(ctx).Execute()

List approval groups



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go/sa-sdk-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApprovalGroupsAPI.ListAuthGroups(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApprovalGroupsAPI.ListAuthGroups``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAuthGroups`: []AuthGroup
	fmt.Fprintf(os.Stdout, "Response from `ApprovalGroupsAPI.ListAuthGroups`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListAuthGroupsRequest struct via the builder pattern


### Return type

[**[]AuthGroup**](AuthGroup.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveUserFromAuthGroup

> RemoveUserFromAuthGroup(ctx, id, userID).Execute()

Remove user from approval group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | User ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ApprovalGroupsAPI.RemoveUserFromAuthGroup(context.Background(), id, userID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApprovalGroupsAPI.RemoveUserFromAuthGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 
**userID** | **string** | User ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveUserFromAuthGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetAuthGroupTags

> SetAuthGroupTags(ctx, id).SetTransactionTagsRequest(setTransactionTagsRequest).Execute()

Set approval group tags



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	setTransactionTagsRequest := *openapiclient.NewSetTransactionTagsRequest() // SetTransactionTagsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ApprovalGroupsAPI.SetAuthGroupTags(context.Background(), id).SetTransactionTagsRequest(setTransactionTagsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApprovalGroupsAPI.SetAuthGroupTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetAuthGroupTagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **setTransactionTagsRequest** | [**SetTransactionTagsRequest**](SetTransactionTagsRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateAuthGroup

> UpdateAuthGroup(ctx, id).AuthGroup(authGroup).Execute()

Update approval group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Approval group ID
	authGroup := *openapiclient.NewAuthGroup("Name_example", "Threshold_example") // AuthGroup | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ApprovalGroupsAPI.UpdateAuthGroup(context.Background(), id).AuthGroup(authGroup).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApprovalGroupsAPI.UpdateAuthGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Approval group ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateAuthGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **authGroup** | [**AuthGroup**](AuthGroup.md) |  | 

### Return type

 (empty response body)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

