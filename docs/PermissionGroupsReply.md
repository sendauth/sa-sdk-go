# PermissionGroupsReply

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Groups** | Pointer to [**[]PermissionGroup**](PermissionGroup.md) |  | [optional] 

## Methods

### NewPermissionGroupsReply

`func NewPermissionGroupsReply() *PermissionGroupsReply`

NewPermissionGroupsReply instantiates a new PermissionGroupsReply object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPermissionGroupsReplyWithDefaults

`func NewPermissionGroupsReplyWithDefaults() *PermissionGroupsReply`

NewPermissionGroupsReplyWithDefaults instantiates a new PermissionGroupsReply object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGroups

`func (o *PermissionGroupsReply) GetGroups() []PermissionGroup`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *PermissionGroupsReply) GetGroupsOk() (*[]PermissionGroup, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *PermissionGroupsReply) SetGroups(v []PermissionGroup)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *PermissionGroupsReply) HasGroups() bool`

HasGroups returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


