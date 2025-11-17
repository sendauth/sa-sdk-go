# Audit

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Subject** | Pointer to **string** | Subject identifier | [optional] 
**Name** | Pointer to **string** | Subject name | [optional] 
**Type** | Pointer to **string** | Subject type | [optional] 
**Actor** | Pointer to **string** | Actor performing the action | [optional] 
**Action** | Pointer to **string** | Action performed | [optional] 
**Extras** | Pointer to **map[string]string** | Additional audit information | [optional] 
**CreatedAt** | Pointer to **time.Time** | Audit entry creation timestamp | [optional] 

## Methods

### NewAudit

`func NewAudit() *Audit`

NewAudit instantiates a new Audit object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuditWithDefaults

`func NewAuditWithDefaults() *Audit`

NewAuditWithDefaults instantiates a new Audit object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSubject

`func (o *Audit) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *Audit) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *Audit) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *Audit) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetName

`func (o *Audit) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Audit) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Audit) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Audit) HasName() bool`

HasName returns a boolean if a field has been set.

### GetType

`func (o *Audit) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Audit) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Audit) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *Audit) HasType() bool`

HasType returns a boolean if a field has been set.

### GetActor

`func (o *Audit) GetActor() string`

GetActor returns the Actor field if non-nil, zero value otherwise.

### GetActorOk

`func (o *Audit) GetActorOk() (*string, bool)`

GetActorOk returns a tuple with the Actor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActor

`func (o *Audit) SetActor(v string)`

SetActor sets Actor field to given value.

### HasActor

`func (o *Audit) HasActor() bool`

HasActor returns a boolean if a field has been set.

### GetAction

`func (o *Audit) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *Audit) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *Audit) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *Audit) HasAction() bool`

HasAction returns a boolean if a field has been set.

### GetExtras

`func (o *Audit) GetExtras() map[string]string`

GetExtras returns the Extras field if non-nil, zero value otherwise.

### GetExtrasOk

`func (o *Audit) GetExtrasOk() (*map[string]string, bool)`

GetExtrasOk returns a tuple with the Extras field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtras

`func (o *Audit) SetExtras(v map[string]string)`

SetExtras sets Extras field to given value.

### HasExtras

`func (o *Audit) HasExtras() bool`

HasExtras returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Audit) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Audit) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Audit) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Audit) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


