# \PermissionGroupsAPI

All URIs are relative to *https://api.sendauth.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreatePermissionGroup**](PermissionGroupsAPI.md#CreatePermissionGroup) | **Post** /api/v1/permission-groups | Create permission group
[**DeletePermissionGroup**](PermissionGroupsAPI.md#DeletePermissionGroup) | **Delete** /api/v1/permission-groups/{id} | Delete permission group
[**ListPermissionGroups**](PermissionGroupsAPI.md#ListPermissionGroups) | **Get** /api/v1/permission-groups | List permission groups
[**RenamePermissionGroup**](PermissionGroupsAPI.md#RenamePermissionGroup) | **Put** /api/v1/permission-groups/{id} | Rename permission group
[**SetPermissionGroupPermissions**](PermissionGroupsAPI.md#SetPermissionGroupPermissions) | **Put** /api/v1/permission-groups/{id}/permissions | Set permission group permissions



## CreatePermissionGroup

> PermissionGroup CreatePermissionGroup(ctx).PermissionGroup(permissionGroup).Execute()

Create permission group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go"
)

func main() {
	permissionGroup := *openapiclient.NewPermissionGroup("Name_example") // PermissionGroup | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PermissionGroupsAPI.CreatePermissionGroup(context.Background()).PermissionGroup(permissionGroup).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PermissionGroupsAPI.CreatePermissionGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreatePermissionGroup`: PermissionGroup
	fmt.Fprintf(os.Stdout, "Response from `PermissionGroupsAPI.CreatePermissionGroup`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreatePermissionGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **permissionGroup** | [**PermissionGroup**](PermissionGroup.md) |  | 

### Return type

[**PermissionGroup**](PermissionGroup.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeletePermissionGroup

> DeletePermissionGroup(ctx, id).Execute()

Delete permission group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.PermissionGroupsAPI.DeletePermissionGroup(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PermissionGroupsAPI.DeletePermissionGroup``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeletePermissionGroupRequest struct via the builder pattern


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


## ListPermissionGroups

> PermissionGroupsReply ListPermissionGroups(ctx).Execute()

List permission groups



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PermissionGroupsAPI.ListPermissionGroups(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PermissionGroupsAPI.ListPermissionGroups``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPermissionGroups`: PermissionGroupsReply
	fmt.Fprintf(os.Stdout, "Response from `PermissionGroupsAPI.ListPermissionGroups`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListPermissionGroupsRequest struct via the builder pattern


### Return type

[**PermissionGroupsReply**](PermissionGroupsReply.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RenamePermissionGroup

> PermissionGroup RenamePermissionGroup(ctx, id).PermissionGroup(permissionGroup).Execute()

Rename permission group



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	permissionGroup := *openapiclient.NewPermissionGroup("Name_example") // PermissionGroup | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PermissionGroupsAPI.RenamePermissionGroup(context.Background(), id).PermissionGroup(permissionGroup).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PermissionGroupsAPI.RenamePermissionGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RenamePermissionGroup`: PermissionGroup
	fmt.Fprintf(os.Stdout, "Response from `PermissionGroupsAPI.RenamePermissionGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRenamePermissionGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **permissionGroup** | [**PermissionGroup**](PermissionGroup.md) |  | 

### Return type

[**PermissionGroup**](PermissionGroup.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetPermissionGroupPermissions

> SetPermissionGroupPermissions(ctx, id).SetPermissionGroupPermissionsRequest(setPermissionGroupPermissionsRequest).Execute()

Set permission group permissions



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/sendauth/sa-sdk-go"
)

func main() {
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	setPermissionGroupPermissionsRequest := *openapiclient.NewSetPermissionGroupPermissionsRequest() // SetPermissionGroupPermissionsRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.PermissionGroupsAPI.SetPermissionGroupPermissions(context.Background(), id).SetPermissionGroupPermissionsRequest(setPermissionGroupPermissionsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PermissionGroupsAPI.SetPermissionGroupPermissions``: %v\n", err)
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

Other parameters are passed through a pointer to a apiSetPermissionGroupPermissionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **setPermissionGroupPermissionsRequest** | [**SetPermissionGroupPermissionsRequest**](SetPermissionGroupPermissionsRequest.md) |  | 

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

