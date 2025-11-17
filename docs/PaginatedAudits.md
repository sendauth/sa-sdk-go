# PaginatedAudits

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Rows** | Pointer to [**[]Audit**](Audit.md) |  | [optional] 
**Total** | Pointer to **int64** | Total number of items | [optional] 

## Methods

### NewPaginatedAudits

`func NewPaginatedAudits() *PaginatedAudits`

NewPaginatedAudits instantiates a new PaginatedAudits object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaginatedAuditsWithDefaults

`func NewPaginatedAuditsWithDefaults() *PaginatedAudits`

NewPaginatedAuditsWithDefaults instantiates a new PaginatedAudits object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRows

`func (o *PaginatedAudits) GetRows() []Audit`

GetRows returns the Rows field if non-nil, zero value otherwise.

### GetRowsOk

`func (o *PaginatedAudits) GetRowsOk() (*[]Audit, bool)`

GetRowsOk returns a tuple with the Rows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRows

`func (o *PaginatedAudits) SetRows(v []Audit)`

SetRows sets Rows field to given value.

### HasRows

`func (o *PaginatedAudits) HasRows() bool`

HasRows returns a boolean if a field has been set.

### GetTotal

`func (o *PaginatedAudits) GetTotal() int64`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *PaginatedAudits) GetTotalOk() (*int64, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *PaginatedAudits) SetTotal(v int64)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *PaginatedAudits) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


