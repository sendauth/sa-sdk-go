# \CompaniesAPI

All URIs are relative to *https://api.sendauth.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateCompany**](CompaniesAPI.md#CreateCompany) | **Post** /api/v1/companies | Create company
[**DeleteCompany**](CompaniesAPI.md#DeleteCompany) | **Delete** /api/v1/companies/{id} | Delete company
[**ListCompanies**](CompaniesAPI.md#ListCompanies) | **Get** /api/v1/companies | List companies
[**UpdateCompany**](CompaniesAPI.md#UpdateCompany) | **Put** /api/v1/companies/{id} | Update company



## CreateCompany

> Company CreateCompany(ctx).Company(company).Execute()

Create company



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
	company := *openapiclient.NewCompany() // Company | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CompaniesAPI.CreateCompany(context.Background()).Company(company).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CompaniesAPI.CreateCompany``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCompany`: Company
	fmt.Fprintf(os.Stdout, "Response from `CompaniesAPI.CreateCompany`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateCompanyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **company** | [**Company**](Company.md) |  | 

### Return type

[**Company**](Company.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteCompany

> DeleteCompany(ctx, id).Execute()

Delete company



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
	r, err := apiClient.CompaniesAPI.DeleteCompany(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CompaniesAPI.DeleteCompany``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteCompanyRequest struct via the builder pattern


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


## ListCompanies

> []Company ListCompanies(ctx).Execute()

List companies



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
	resp, r, err := apiClient.CompaniesAPI.ListCompanies(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CompaniesAPI.ListCompanies``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCompanies`: []Company
	fmt.Fprintf(os.Stdout, "Response from `CompaniesAPI.ListCompanies`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListCompaniesRequest struct via the builder pattern


### Return type

[**[]Company**](Company.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateCompany

> Company UpdateCompany(ctx, id).Company(company).Execute()

Update company



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
	company := *openapiclient.NewCompany() // Company | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CompaniesAPI.UpdateCompany(context.Background(), id).Company(company).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CompaniesAPI.UpdateCompany``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateCompany`: Company
	fmt.Fprintf(os.Stdout, "Response from `CompaniesAPI.UpdateCompany`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateCompanyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **company** | [**Company**](Company.md) |  | 

### Return type

[**Company**](Company.md)

### Authorization

[basic](../README.md#basic)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

