# Transaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Transaction identifier | [optional] 
**Subject** | Pointer to **string** | Subject user ID | [optional] 
**SubjectName** | Pointer to **string** | Subject user name | [optional] 
**State** | Pointer to **string** | Transaction state | [optional] 
**CompletedAt** | Pointer to **time.Time** | Transaction completion timestamp | [optional] 
**Requestor** | Pointer to **string** | Transaction requestor | [optional] 
**Context** | Pointer to **string** | Transaction context | [optional] 
**CreatedAt** | Pointer to **time.Time** | Transaction creation timestamp | [optional] 
**ExpiresAt** | Pointer to **time.Time** | Transaction expiration timestamp | [optional] 
**Message** | Pointer to **string** | Transaction message | [optional] 
**UserMessage** | Pointer to **string** | User-provided message | [optional] 

## Methods

### NewTransaction

`func NewTransaction() *Transaction`

NewTransaction instantiates a new Transaction object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTransactionWithDefaults

`func NewTransactionWithDefaults() *Transaction`

NewTransactionWithDefaults instantiates a new Transaction object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Transaction) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Transaction) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Transaction) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *Transaction) HasId() bool`

HasId returns a boolean if a field has been set.

### GetSubject

`func (o *Transaction) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *Transaction) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *Transaction) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *Transaction) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetSubjectName

`func (o *Transaction) GetSubjectName() string`

GetSubjectName returns the SubjectName field if non-nil, zero value otherwise.

### GetSubjectNameOk

`func (o *Transaction) GetSubjectNameOk() (*string, bool)`

GetSubjectNameOk returns a tuple with the SubjectName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubjectName

`func (o *Transaction) SetSubjectName(v string)`

SetSubjectName sets SubjectName field to given value.

### HasSubjectName

`func (o *Transaction) HasSubjectName() bool`

HasSubjectName returns a boolean if a field has been set.

### GetState

`func (o *Transaction) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *Transaction) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *Transaction) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *Transaction) HasState() bool`

HasState returns a boolean if a field has been set.

### GetCompletedAt

`func (o *Transaction) GetCompletedAt() time.Time`

GetCompletedAt returns the CompletedAt field if non-nil, zero value otherwise.

### GetCompletedAtOk

`func (o *Transaction) GetCompletedAtOk() (*time.Time, bool)`

GetCompletedAtOk returns a tuple with the CompletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedAt

`func (o *Transaction) SetCompletedAt(v time.Time)`

SetCompletedAt sets CompletedAt field to given value.

### HasCompletedAt

`func (o *Transaction) HasCompletedAt() bool`

HasCompletedAt returns a boolean if a field has been set.

### GetRequestor

`func (o *Transaction) GetRequestor() string`

GetRequestor returns the Requestor field if non-nil, zero value otherwise.

### GetRequestorOk

`func (o *Transaction) GetRequestorOk() (*string, bool)`

GetRequestorOk returns a tuple with the Requestor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestor

`func (o *Transaction) SetRequestor(v string)`

SetRequestor sets Requestor field to given value.

### HasRequestor

`func (o *Transaction) HasRequestor() bool`

HasRequestor returns a boolean if a field has been set.

### GetContext

`func (o *Transaction) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *Transaction) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *Transaction) SetContext(v string)`

SetContext sets Context field to given value.

### HasContext

`func (o *Transaction) HasContext() bool`

HasContext returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Transaction) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Transaction) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Transaction) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Transaction) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetExpiresAt

`func (o *Transaction) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *Transaction) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *Transaction) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *Transaction) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### GetMessage

`func (o *Transaction) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *Transaction) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *Transaction) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *Transaction) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetUserMessage

`func (o *Transaction) GetUserMessage() string`

GetUserMessage returns the UserMessage field if non-nil, zero value otherwise.

### GetUserMessageOk

`func (o *Transaction) GetUserMessageOk() (*string, bool)`

GetUserMessageOk returns a tuple with the UserMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserMessage

`func (o *Transaction) SetUserMessage(v string)`

SetUserMessage sets UserMessage field to given value.

### HasUserMessage

`func (o *Transaction) HasUserMessage() bool`

HasUserMessage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


