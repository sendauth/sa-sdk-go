# Query

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Page** | Pointer to **int32** | Page number | [optional] 
**PerPage** | Pointer to **int32** | Items per page | [optional] 
**Q** | Pointer to **string** | Search query | [optional] 
**Permission** | Pointer to **string** | Filter by permission | [optional] 
**SortBy** | Pointer to **string** | Sort field | [optional] 
**SortDir** | Pointer to **string** | Sort direction | [optional] 

## Methods

### NewQuery

`func NewQuery() *Query`

NewQuery instantiates a new Query object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewQueryWithDefaults

`func NewQueryWithDefaults() *Query`

NewQueryWithDefaults instantiates a new Query object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPage

`func (o *Query) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *Query) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *Query) SetPage(v int32)`

SetPage sets Page field to given value.

### HasPage

`func (o *Query) HasPage() bool`

HasPage returns a boolean if a field has been set.

### GetPerPage

`func (o *Query) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *Query) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *Query) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *Query) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetQ

`func (o *Query) GetQ() string`

GetQ returns the Q field if non-nil, zero value otherwise.

### GetQOk

`func (o *Query) GetQOk() (*string, bool)`

GetQOk returns a tuple with the Q field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQ

`func (o *Query) SetQ(v string)`

SetQ sets Q field to given value.

### HasQ

`func (o *Query) HasQ() bool`

HasQ returns a boolean if a field has been set.

### GetPermission

`func (o *Query) GetPermission() string`

GetPermission returns the Permission field if non-nil, zero value otherwise.

### GetPermissionOk

`func (o *Query) GetPermissionOk() (*string, bool)`

GetPermissionOk returns a tuple with the Permission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPermission

`func (o *Query) SetPermission(v string)`

SetPermission sets Permission field to given value.

### HasPermission

`func (o *Query) HasPermission() bool`

HasPermission returns a boolean if a field has been set.

### GetSortBy

`func (o *Query) GetSortBy() string`

GetSortBy returns the SortBy field if non-nil, zero value otherwise.

### GetSortByOk

`func (o *Query) GetSortByOk() (*string, bool)`

GetSortByOk returns a tuple with the SortBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortBy

`func (o *Query) SetSortBy(v string)`

SetSortBy sets SortBy field to given value.

### HasSortBy

`func (o *Query) HasSortBy() bool`

HasSortBy returns a boolean if a field has been set.

### GetSortDir

`func (o *Query) GetSortDir() string`

GetSortDir returns the SortDir field if non-nil, zero value otherwise.

### GetSortDirOk

`func (o *Query) GetSortDirOk() (*string, bool)`

GetSortDirOk returns a tuple with the SortDir field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortDir

`func (o *Query) SetSortDir(v string)`

SetSortDir sets SortDir field to given value.

### HasSortDir

`func (o *Query) HasSortDir() bool`

HasSortDir returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


