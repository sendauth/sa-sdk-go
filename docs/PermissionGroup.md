# PermissionGroup

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Permission group identifier | [optional] 
**Name** | **string** | Permission group name | 
**Permissions** | Pointer to **[]string** | Permissions in this group | [optional] 

## Methods

### NewPermissionGroup

`func NewPermissionGroup(name string, ) *PermissionGroup`

NewPermissionGroup instantiates a new PermissionGroup object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPermissionGroupWithDefaults

`func NewPermissionGroupWithDefaults() *PermissionGroup`

NewPermissionGroupWithDefaults instantiates a new PermissionGroup object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *PermissionGroup) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PermissionGroup) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PermissionGroup) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *PermissionGroup) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *PermissionGroup) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PermissionGroup) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PermissionGroup) SetName(v string)`

SetName sets Name field to given value.


### GetPermissions

`func (o *PermissionGroup) GetPermissions() []string`

GetPermissions returns the Permissions field if non-nil, zero value otherwise.

### GetPermissionsOk

`func (o *PermissionGroup) GetPermissionsOk() (*[]string, bool)`

GetPermissionsOk returns a tuple with the Permissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPermissions

`func (o *PermissionGroup) SetPermissions(v []string)`

SetPermissions sets Permissions field to given value.

### HasPermissions

`func (o *PermissionGroup) HasPermissions() bool`

HasPermissions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


