# \TransactionsAPI

All URIs are relative to *https://api.sendauth.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelTransaction**](TransactionsAPI.md#CancelTransaction) | **Delete** /api/v1/transactions/{txID}/cancel | Cancel transaction
[**CheckTransactionStatus**](TransactionsAPI.md#CheckTransactionStatus) | **Get** /api/v1/transactions/{txID}/check | Check transaction status
[**GetTransactionHistory**](TransactionsAPI.md#GetTransactionHistory) | **Get** /api/v1/transactions/{txID}/history | Get transaction history
[**ListTransactions**](TransactionsAPI.md#ListTransactions) | **Get** /api/v1/transactions | List transactions
[**SetTransactionTags**](TransactionsAPI.md#SetTransactionTags) | **Put** /api/v1/transactions/{txID}/tags | Set transaction tags



## CancelTransaction

> CancelTransaction(ctx, txID).Execute()

Cancel transaction



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
	txID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.TransactionsAPI.CancelTransaction(context.Background(), txID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TransactionsAPI.CancelTransaction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**txID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelTransactionRequest struct via the builder pattern


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


## CheckTransactionStatus

> CheckTransactionStatus200Response CheckTransactionStatus(ctx, txID).Execute()

Check transaction status



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
	txID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TransactionsAPI.CheckTransactionStatus(context.Background(), txID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TransactionsAPI.CheckTransactionStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CheckTransactionStatus`: CheckTransactionStatus200Response
	fmt.Fprintf(os.Stdout, "Response from `TransactionsAPI.CheckTransactionStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**txID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCheckTransactionStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CheckTransactionStatus200Response**](CheckTransactionStatus200Response.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTransactionHistory

> Transaction GetTransactionHistory(ctx, txID).Execute()

Get transaction history



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
	txID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TransactionsAPI.GetTransactionHistory(context.Background(), txID).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TransactionsAPI.GetTransactionHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTransactionHistory`: Transaction
	fmt.Fprintf(os.Stdout, "Response from `TransactionsAPI.GetTransactionHistory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**txID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTransactionHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Transaction**](Transaction.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTransactions

> PaginatedTransactions ListTransactions(ctx).Page(page).PerPage(perPage).Q(q).Execute()

List transactions



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TransactionsAPI.ListTransactions(context.Background()).Page(page).PerPage(perPage).Q(q).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TransactionsAPI.ListTransactions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTransactions`: PaginatedTransactions
	fmt.Fprintf(os.Stdout, "Response from `TransactionsAPI.ListTransactions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListTransactionsRequest struct via the builder pattern


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


## SetTransactionTags

> SetTransactionTags(ctx, txID).SetTransactionTagsRequest(setTransactionTagsRequest).Execute()

Set transaction tags



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
	txID := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	setTransactionTagsRequest := *openapiclient.NewSetTransactionTagsRequest() // SetTransactionTagsRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.TransactionsAPI.SetTransactionTags(context.Background(), txID).SetTransactionTagsRequest(setTransactionTagsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TransactionsAPI.SetTransactionTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**txID** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetTransactionTagsRequest struct via the builder pattern


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

