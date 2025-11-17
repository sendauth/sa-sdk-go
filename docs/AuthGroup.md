# AuthGroup

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | The unique identifier of the approval group | [optional] 
**Name** | **string** | The name of the approval group | 
**Threshold** | **string** | The threshold for the approval group | 
**Description** | Pointer to **string** |  | [optional] 
**Users** | Pointer to [**[]AuthGroupMember**](AuthGroupMember.md) |  | [optional] 

## Methods

### NewAuthGroup

`func NewAuthGroup(name string, threshold string, ) *AuthGroup`

NewAuthGroup instantiates a new AuthGroup object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthGroupWithDefaults

`func NewAuthGroupWithDefaults() *AuthGroup`

NewAuthGroupWithDefaults instantiates a new AuthGroup object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AuthGroup) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AuthGroup) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AuthGroup) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *AuthGroup) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *AuthGroup) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AuthGroup) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AuthGroup) SetName(v string)`

SetName sets Name field to given value.


### GetThreshold

`func (o *AuthGroup) GetThreshold() string`

GetThreshold returns the Threshold field if non-nil, zero value otherwise.

### GetThresholdOk

`func (o *AuthGroup) GetThresholdOk() (*string, bool)`

GetThresholdOk returns a tuple with the Threshold field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThreshold

`func (o *AuthGroup) SetThreshold(v string)`

SetThreshold sets Threshold field to given value.


### GetDescription

`func (o *AuthGroup) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *AuthGroup) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *AuthGroup) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *AuthGroup) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetUsers

`func (o *AuthGroup) GetUsers() []AuthGroupMember`

GetUsers returns the Users field if non-nil, zero value otherwise.

### GetUsersOk

`func (o *AuthGroup) GetUsersOk() (*[]AuthGroupMember, bool)`

GetUsersOk returns a tuple with the Users field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsers

`func (o *AuthGroup) SetUsers(v []AuthGroupMember)`

SetUsers sets Users field to given value.

### HasUsers

`func (o *AuthGroup) HasUsers() bool`

HasUsers returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


