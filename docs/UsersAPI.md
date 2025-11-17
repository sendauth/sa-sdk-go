# \UsersAPI

All URIs are relative to *https://api.sendauth.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AuthenticateUser**](UsersAPI.md#AuthenticateUser) | **Post** /api/v1/users/{userID}/authenticate | Authenticate user
[**CreateUser**](UsersAPI.md#CreateUser) | **Post** /api/v1/users | Create user
[**DeleteUser**](UsersAPI.md#DeleteUser) | **Delete** /api/v1/users/{userID} | Delete user
[**DestroyUser**](UsersAPI.md#DestroyUser) | **Delete** /api/v1/users/deleted/{userID} | Permanently delete user
[**GetUser**](UsersAPI.md#GetUser) | **Get** /api/v1/users/{userID} | Get user
[**GetUserAudits**](UsersAPI.md#GetUserAudits) | **Get** /api/v1/users/{userID}/audits | Get user audits
[**GetUserTransactions**](UsersAPI.md#GetUserTransactions) | **Get** /api/v1/users/{userID}/transactions | Get user transactions
[**ListDeletedUsers**](UsersAPI.md#ListDeletedUsers) | **Get** /api/v1/users/deleted | List deleted users
[**ListUsers**](UsersAPI.md#ListUsers) | **Get** /api/v1/users | List users
[**RegisterUser**](UsersAPI.md#RegisterUser) | **Post** /api/v1/users/{userID}/register | Register user
[**RemoveUserPasskey**](UsersAPI.md#RemoveUserPasskey) | **Delete** /api/v1/users/{userID}/passkey | Remove user passkey
[**RestoreUser**](UsersAPI.md#RestoreUser) | **Put** /api/v1/users/deleted/{userID} | Restore deleted user
[**SetUserTags**](UsersAPI.md#SetUserTags) | **Put** /api/v1/users/{userID}/tags | Set user tags
[**UpdateUser**](UsersAPI.md#UpdateUser) | **Put** /api/v1/users/{userID} | Update user



## AuthenticateUser

> TX AuthenticateUser(ctx, userID).WebTX(webTX).Execute()

Authenticate user



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	webTX := *openapiclient.NewWebTX() // WebTX |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.AuthenticateUser(context.Background(), userID).WebTX(webTX).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.AuthenticateUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthenticateUser`: TX
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.AuthenticateUser`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAuthenticateUserRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **webTX** | [**WebTX**](WebTX.md) |  | 

### Return type

[**TX**](TX.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateUser

> User CreateUser(ctx).User(user).Execute()

Create user



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
	user := *openapiclient.NewUser("FirstName_example", "LastName_example") // User | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.CreateUser(context.Background()).User(user).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.CreateUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateUser`: User
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.CreateUser`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateUserRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | [**User**](User.md) |  | 

### Return type

[**User**](User.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteUser

> DeleteUser(ctx, userID).Execute()

Delete user



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.UsersAPI.DeleteUser(context.Background(), userID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.DeleteUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteUserRequest struct via the builder pattern


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


## DestroyUser

> DestroyUser(ctx, userID).Execute()

Permanently delete user



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.UsersAPI.DestroyUser(context.Background(), userID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.DestroyUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDestroyUserRequest struct via the builder pattern


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


## GetUser

> User GetUser(ctx, userID).Execute()

Get user



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.GetUser(context.Background(), userID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.GetUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUser`: User
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.GetUser`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**User**](User.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserAudits

> PaginatedAudits GetUserAudits(ctx, userID).Page(page).PerPage(perPage).Q(q).Execute()

Get user audits



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	page := int32(56) // int32 |  (optional)
	perPage := int32(56) // int32 |  (optional)
	q := "q_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.GetUserAudits(context.Background(), userID).Page(page).PerPage(perPage).Q(q).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.GetUserAudits``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserAudits`: PaginatedAudits
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.GetUserAudits`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserAuditsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | 
 **perPage** | **int32** |  | 
 **q** | **string** |  | 

### Return type

[**PaginatedAudits**](PaginatedAudits.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUserTransactions

> PaginatedTransactions GetUserTransactions(ctx, userID).Page(page).PerPage(perPage).Q(q).Execute()

Get user transactions



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	page := int32(56) // int32 |  (optional)
	perPage := int32(56) // int32 |  (optional)
	q := "q_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.GetUserTransactions(context.Background(), userID).Page(page).PerPage(perPage).Q(q).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.GetUserTransactions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUserTransactions`: PaginatedTransactions
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.GetUserTransactions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetUserTransactionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | 
 **perPage** | **int32** |  | 
 **q** | **string** |  | 

### Return type

[**PaginatedTransactions**](PaginatedTransactions.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDeletedUsers

> PaginatedUsers ListDeletedUsers(ctx).Page(page).PerPage(perPage).Q(q).Permission(permission).Execute()

List deleted users



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
	page := int32(56) // int32 |  (optional)
	perPage := int32(56) // int32 |  (optional)
	q := "q_example" // string |  (optional)
	permission := "permission_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.ListDeletedUsers(context.Background()).Page(page).PerPage(perPage).Q(q).Permission(permission).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.ListDeletedUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDeletedUsers`: PaginatedUsers
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.ListDeletedUsers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDeletedUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int32** |  | 
 **perPage** | **int32** |  | 
 **q** | **string** |  | 
 **permission** | **string** |  | 

### Return type

[**PaginatedUsers**](PaginatedUsers.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListUsers

> PaginatedUsers ListUsers(ctx).Page(page).PerPage(perPage).Q(q).Permission(permission).SortBy(sortBy).SortDir(sortDir).Execute()

List users



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
	page := int32(56) // int32 |  (optional)
	perPage := int32(56) // int32 |  (optional)
	q := "q_example" // string |  (optional)
	permission := "permission_example" // string |  (optional)
	sortBy := "sortBy_example" // string |  (optional)
	sortDir := "sortDir_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.ListUsers(context.Background()).Page(page).PerPage(perPage).Q(q).Permission(permission).SortBy(sortBy).SortDir(sortDir).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.ListUsers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListUsers`: PaginatedUsers
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.ListUsers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListUsersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int32** |  | 
 **perPage** | **int32** |  | 
 **q** | **string** |  | 
 **permission** | **string** |  | 
 **sortBy** | **string** |  | 
 **sortDir** | **string** |  | 

### Return type

[**PaginatedUsers**](PaginatedUsers.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegisterUser

> TX RegisterUser(ctx, userID).Execute()

Register user



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.RegisterUser(context.Background(), userID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.RegisterUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterUser`: TX
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.RegisterUser`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRegisterUserRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TX**](TX.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveUserPasskey

> RemoveUserPasskey(ctx, userID).Execute()

Remove user passkey



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.UsersAPI.RemoveUserPasskey(context.Background(), userID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.RemoveUserPasskey``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveUserPasskeyRequest struct via the builder pattern


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


## RestoreUser

> RestoreUser(ctx, userID).Execute()

Restore deleted user



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.UsersAPI.RestoreUser(context.Background(), userID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.RestoreUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRestoreUserRequest struct via the builder pattern


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


## SetUserTags

> SetUserTags(ctx, userID).TagsRequest(tagsRequest).Execute()

Set user tags



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	tagsRequest := *openapiclient.NewTagsRequest() // TagsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.UsersAPI.SetUserTags(context.Background(), userID).TagsRequest(tagsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.SetUserTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetUserTagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **tagsRequest** | [**TagsRequest**](TagsRequest.md) |  | 

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


## UpdateUser

> User UpdateUser(ctx, userID).User(user).Execute()

Update user



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
	userID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	user := *openapiclient.NewUser("FirstName_example", "LastName_example") // User | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UsersAPI.UpdateUser(context.Background(), userID).User(user).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UsersAPI.UpdateUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateUser`: User
	fmt.Fprintf(os.Stdout, "Response from `UsersAPI.UpdateUser`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**userID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateUserRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **user** | [**User**](User.md) |  | 

### Return type

[**User**](User.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

