# \RoutingRulesAPI

All URIs are relative to *https://app.sendauth.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Authorize**](RoutingRulesAPI.md#Authorize) | **Post** /api/v1/authorize | Authorize a request
[**CreateRoutingRule**](RoutingRulesAPI.md#CreateRoutingRule) | **Post** /api/v1/tag-routing-rules | Create routing rule
[**DeleteRoutingRule**](RoutingRulesAPI.md#DeleteRoutingRule) | **Delete** /api/v1/tag-routing-rules/{id} | Delete routing rule
[**GetRoutingRule**](RoutingRulesAPI.md#GetRoutingRule) | **Get** /api/v1/tag-routing-rules/{id} | Get routing rules
[**ListRoutingRules**](RoutingRulesAPI.md#ListRoutingRules) | **Get** /api/v1/tag-routing-rules | Get routing rules
[**UpdateRoutingRule**](RoutingRulesAPI.md#UpdateRoutingRule) | **Put** /api/v1/tag-routing-rules/{id} | Update routing rule



## Authorize

> AuthorizeReply Authorize(ctx).AuthorizeRequest(authorizeRequest).Execute()

Authorize a request



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
	authorizeRequest := *openapiclient.NewAuthorizeRequest("Message_example", map[string]string{"key": "Inner_example"}) // AuthorizeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoutingRulesAPI.Authorize(context.Background()).AuthorizeRequest(authorizeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutingRulesAPI.Authorize``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Authorize`: AuthorizeReply
	fmt.Fprintf(os.Stdout, "Response from `RoutingRulesAPI.Authorize`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAuthorizeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorizeRequest** | [**AuthorizeRequest**](AuthorizeRequest.md) |  | 

### Return type

[**AuthorizeReply**](AuthorizeReply.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateRoutingRule

> IDReply CreateRoutingRule(ctx).RoutingRule(routingRule).Execute()

Create routing rule



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
	routingRule := *openapiclient.NewRoutingRule("TagName_example", "TagValue_example", "TargetType_example", "TargetId_example") // RoutingRule | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoutingRulesAPI.CreateRoutingRule(context.Background()).RoutingRule(routingRule).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutingRulesAPI.CreateRoutingRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRoutingRule`: IDReply
	fmt.Fprintf(os.Stdout, "Response from `RoutingRulesAPI.CreateRoutingRule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateRoutingRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **routingRule** | [**RoutingRule**](RoutingRule.md) |  | 

### Return type

[**IDReply**](IDReply.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteRoutingRule

> DeleteRoutingRule(ctx, id).Execute()

Delete routing rule



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
	id := "id_example" // string | Routing rule ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RoutingRulesAPI.DeleteRoutingRule(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutingRulesAPI.DeleteRoutingRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Routing rule ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteRoutingRuleRequest struct via the builder pattern


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


## GetRoutingRule

> RoutingRule GetRoutingRule(ctx, id).Execute()

Get routing rules



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
	id := "id_example" // string | Routing rule ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.RoutingRulesAPI.GetRoutingRule(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutingRulesAPI.GetRoutingRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRoutingRule`: RoutingRule
	fmt.Fprintf(os.Stdout, "Response from `RoutingRulesAPI.GetRoutingRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Routing rule ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetRoutingRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**RoutingRule**](RoutingRule.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListRoutingRules

> []RoutingRule ListRoutingRules(ctx).Execute()

Get routing rules



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
	resp, r, err := apiClient.RoutingRulesAPI.ListRoutingRules(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutingRulesAPI.ListRoutingRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListRoutingRules`: []RoutingRule
	fmt.Fprintf(os.Stdout, "Response from `RoutingRulesAPI.ListRoutingRules`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListRoutingRulesRequest struct via the builder pattern


### Return type

[**[]RoutingRule**](RoutingRule.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateRoutingRule

> UpdateRoutingRule(ctx, id).RoutingRule(routingRule).Execute()

Update routing rule



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
	id := "id_example" // string | Routing rule ID
	routingRule := *openapiclient.NewRoutingRule("TagName_example", "TagValue_example", "TargetType_example", "TargetId_example") // RoutingRule | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.RoutingRulesAPI.UpdateRoutingRule(context.Background(), id).RoutingRule(routingRule).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `RoutingRulesAPI.UpdateRoutingRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Routing rule ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateRoutingRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **routingRule** | [**RoutingRule**](RoutingRule.md) |  | 

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

