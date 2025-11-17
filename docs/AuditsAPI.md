# \AuditsAPI

All URIs are relative to *https://api.sendauth.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListAudits**](AuditsAPI.md#ListAudits) | **Get** /api/v1/audits | List audits



## ListAudits

> PaginatedAudits ListAudits(ctx).Page(page).PerPage(perPage).Q(q).Execute()

List audits



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
	resp, r, err := apiClient.AuditsAPI.ListAudits(context.Background()).Page(page).PerPage(perPage).Q(q).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuditsAPI.ListAudits``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAudits`: PaginatedAudits
	fmt.Fprintf(os.Stdout, "Response from `AuditsAPI.ListAudits`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAuditsRequest struct via the builder pattern


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

