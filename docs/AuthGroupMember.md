# AuthGroupMember

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | The unique identifier of the user | [optional] 
**Email** | Pointer to **string** | The email address of the user | [optional] 
**FirstName** | Pointer to **string** | The first name of the user | [optional] 
**LastName** | Pointer to **string** | The last name of the user | [optional] 

## Methods

### NewAuthGroupMember

`func NewAuthGroupMember() *AuthGroupMember`

NewAuthGroupMember instantiates a new AuthGroupMember object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthGroupMemberWithDefaults

`func NewAuthGroupMemberWithDefaults() *AuthGroupMember`

NewAuthGroupMemberWithDefaults instantiates a new AuthGroupMember object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AuthGroupMember) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AuthGroupMember) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AuthGroupMember) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *AuthGroupMember) HasId() bool`

HasId returns a boolean if a field has been set.

### GetEmail

`func (o *AuthGroupMember) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *AuthGroupMember) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *AuthGroupMember) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *AuthGroupMember) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetFirstName

`func (o *AuthGroupMember) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *AuthGroupMember) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *AuthGroupMember) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.

### HasFirstName

`func (o *AuthGroupMember) HasFirstName() bool`

HasFirstName returns a boolean if a field has been set.

### GetLastName

`func (o *AuthGroupMember) GetLastName() string`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *AuthGroupMember) GetLastNameOk() (*string, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *AuthGroupMember) SetLastName(v string)`

SetLastName sets LastName field to given value.

### HasLastName

`func (o *AuthGroupMember) HasLastName() bool`

HasLastName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


