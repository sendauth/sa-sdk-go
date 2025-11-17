# PaginatedUsers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Rows** | Pointer to [**[]User**](User.md) |  | [optional] 
**Total** | Pointer to **int64** | Total number of items | [optional] 

## Methods

### NewPaginatedUsers

`func NewPaginatedUsers() *PaginatedUsers`

NewPaginatedUsers instantiates a new PaginatedUsers object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaginatedUsersWithDefaults

`func NewPaginatedUsersWithDefaults() *PaginatedUsers`

NewPaginatedUsersWithDefaults instantiates a new PaginatedUsers object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRows

`func (o *PaginatedUsers) GetRows() []User`

GetRows returns the Rows field if non-nil, zero value otherwise.

### GetRowsOk

`func (o *PaginatedUsers) GetRowsOk() (*[]User, bool)`

GetRowsOk returns a tuple with the Rows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRows

`func (o *PaginatedUsers) SetRows(v []User)`

SetRows sets Rows field to given value.

### HasRows

`func (o *PaginatedUsers) HasRows() bool`

HasRows returns a boolean if a field has been set.

### GetTotal

`func (o *PaginatedUsers) GetTotal() int64`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *PaginatedUsers) GetTotalOk() (*int64, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *PaginatedUsers) SetTotal(v int64)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *PaginatedUsers) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


