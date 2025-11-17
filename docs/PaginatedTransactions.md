# PaginatedTransactions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Rows** | Pointer to [**[]Transaction**](Transaction.md) |  | [optional] 
**Total** | Pointer to **int64** | Total number of items | [optional] 

## Methods

### NewPaginatedTransactions

`func NewPaginatedTransactions() *PaginatedTransactions`

NewPaginatedTransactions instantiates a new PaginatedTransactions object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaginatedTransactionsWithDefaults

`func NewPaginatedTransactionsWithDefaults() *PaginatedTransactions`

NewPaginatedTransactionsWithDefaults instantiates a new PaginatedTransactions object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRows

`func (o *PaginatedTransactions) GetRows() []Transaction`

GetRows returns the Rows field if non-nil, zero value otherwise.

### GetRowsOk

`func (o *PaginatedTransactions) GetRowsOk() (*[]Transaction, bool)`

GetRowsOk returns a tuple with the Rows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRows

`func (o *PaginatedTransactions) SetRows(v []Transaction)`

SetRows sets Rows field to given value.

### HasRows

`func (o *PaginatedTransactions) HasRows() bool`

HasRows returns a boolean if a field has been set.

### GetTotal

`func (o *PaginatedTransactions) GetTotal() int64`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *PaginatedTransactions) GetTotalOk() (*int64, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *PaginatedTransactions) SetTotal(v int64)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *PaginatedTransactions) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


