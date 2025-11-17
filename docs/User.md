# User

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique user identifier | [optional] [readonly] 
**Role** | Pointer to **string** | User role | [optional] 
**Username** | Pointer to **string** | Display username | [optional] [readonly] 
**FirstName** | **string** | User first name | 
**LastName** | **string** | User last name | 
**Email** | Pointer to **string** | User email address | [optional] 
**Phone** | Pointer to **string** | User phone number | [optional] 
**Company** | Pointer to [**Company**](Company.md) |  | [optional] 
**Permissions** | Pointer to **[]string** | User direct permissions | [optional] 
**GroupPermissions** | Pointer to **[]string** | Permissions from groups | [optional] 
**PermissionGroups** | Pointer to **[]string** | Permission group IDs | [optional] 
**MessagingPreference** | Pointer to **string** | User messaging preference | [optional] 
**HasPasskeys** | Pointer to **bool** | Whether user has passkeys configured | [optional] [readonly] 
**CreatedAt** | Pointer to **time.Time** | User creation timestamp | [optional] [readonly] 
**LastAuthenticated** | Pointer to **time.Time** | Last authentication timestamp | [optional] [readonly] 

## Methods

### NewUser

`func NewUser(firstName string, lastName string, ) *User`

NewUser instantiates a new User object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserWithDefaults

`func NewUserWithDefaults() *User`

NewUserWithDefaults instantiates a new User object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *User) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *User) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *User) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *User) HasId() bool`

HasId returns a boolean if a field has been set.

### GetRole

`func (o *User) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *User) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *User) SetRole(v string)`

SetRole sets Role field to given value.

### HasRole

`func (o *User) HasRole() bool`

HasRole returns a boolean if a field has been set.

### GetUsername

`func (o *User) GetUsername() string`

GetUsername returns the Username field if non-nil, zero value otherwise.

### GetUsernameOk

`func (o *User) GetUsernameOk() (*string, bool)`

GetUsernameOk returns a tuple with the Username field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsername

`func (o *User) SetUsername(v string)`

SetUsername sets Username field to given value.

### HasUsername

`func (o *User) HasUsername() bool`

HasUsername returns a boolean if a field has been set.

### GetFirstName

`func (o *User) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *User) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *User) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.


### GetLastName

`func (o *User) GetLastName() string`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *User) GetLastNameOk() (*string, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *User) SetLastName(v string)`

SetLastName sets LastName field to given value.


### GetEmail

`func (o *User) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *User) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *User) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *User) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetPhone

`func (o *User) GetPhone() string`

GetPhone returns the Phone field if non-nil, zero value otherwise.

### GetPhoneOk

`func (o *User) GetPhoneOk() (*string, bool)`

GetPhoneOk returns a tuple with the Phone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhone

`func (o *User) SetPhone(v string)`

SetPhone sets Phone field to given value.

### HasPhone

`func (o *User) HasPhone() bool`

HasPhone returns a boolean if a field has been set.

### GetCompany

`func (o *User) GetCompany() Company`

GetCompany returns the Company field if non-nil, zero value otherwise.

### GetCompanyOk

`func (o *User) GetCompanyOk() (*Company, bool)`

GetCompanyOk returns a tuple with the Company field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompany

`func (o *User) SetCompany(v Company)`

SetCompany sets Company field to given value.

### HasCompany

`func (o *User) HasCompany() bool`

HasCompany returns a boolean if a field has been set.

### GetPermissions

`func (o *User) GetPermissions() []string`

GetPermissions returns the Permissions field if non-nil, zero value otherwise.

### GetPermissionsOk

`func (o *User) GetPermissionsOk() (*[]string, bool)`

GetPermissionsOk returns a tuple with the Permissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPermissions

`func (o *User) SetPermissions(v []string)`

SetPermissions sets Permissions field to given value.

### HasPermissions

`func (o *User) HasPermissions() bool`

HasPermissions returns a boolean if a field has been set.

### GetGroupPermissions

`func (o *User) GetGroupPermissions() []string`

GetGroupPermissions returns the GroupPermissions field if non-nil, zero value otherwise.

### GetGroupPermissionsOk

`func (o *User) GetGroupPermissionsOk() (*[]string, bool)`

GetGroupPermissionsOk returns a tuple with the GroupPermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroupPermissions

`func (o *User) SetGroupPermissions(v []string)`

SetGroupPermissions sets GroupPermissions field to given value.

### HasGroupPermissions

`func (o *User) HasGroupPermissions() bool`

HasGroupPermissions returns a boolean if a field has been set.

### GetPermissionGroups

`func (o *User) GetPermissionGroups() []string`

GetPermissionGroups returns the PermissionGroups field if non-nil, zero value otherwise.

### GetPermissionGroupsOk

`func (o *User) GetPermissionGroupsOk() (*[]string, bool)`

GetPermissionGroupsOk returns a tuple with the PermissionGroups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPermissionGroups

`func (o *User) SetPermissionGroups(v []string)`

SetPermissionGroups sets PermissionGroups field to given value.

### HasPermissionGroups

`func (o *User) HasPermissionGroups() bool`

HasPermissionGroups returns a boolean if a field has been set.

### GetMessagingPreference

`func (o *User) GetMessagingPreference() string`

GetMessagingPreference returns the MessagingPreference field if non-nil, zero value otherwise.

### GetMessagingPreferenceOk

`func (o *User) GetMessagingPreferenceOk() (*string, bool)`

GetMessagingPreferenceOk returns a tuple with the MessagingPreference field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagingPreference

`func (o *User) SetMessagingPreference(v string)`

SetMessagingPreference sets MessagingPreference field to given value.

### HasMessagingPreference

`func (o *User) HasMessagingPreference() bool`

HasMessagingPreference returns a boolean if a field has been set.

### GetHasPasskeys

`func (o *User) GetHasPasskeys() bool`

GetHasPasskeys returns the HasPasskeys field if non-nil, zero value otherwise.

### GetHasPasskeysOk

`func (o *User) GetHasPasskeysOk() (*bool, bool)`

GetHasPasskeysOk returns a tuple with the HasPasskeys field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasPasskeys

`func (o *User) SetHasPasskeys(v bool)`

SetHasPasskeys sets HasPasskeys field to given value.

### HasHasPasskeys

`func (o *User) HasHasPasskeys() bool`

HasHasPasskeys returns a boolean if a field has been set.

### GetCreatedAt

`func (o *User) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *User) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *User) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *User) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastAuthenticated

`func (o *User) GetLastAuthenticated() time.Time`

GetLastAuthenticated returns the LastAuthenticated field if non-nil, zero value otherwise.

### GetLastAuthenticatedOk

`func (o *User) GetLastAuthenticatedOk() (*time.Time, bool)`

GetLastAuthenticatedOk returns a tuple with the LastAuthenticated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastAuthenticated

`func (o *User) SetLastAuthenticated(v time.Time)`

SetLastAuthenticated sets LastAuthenticated field to given value.

### HasLastAuthenticated

`func (o *User) HasLastAuthenticated() bool`

HasLastAuthenticated returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


