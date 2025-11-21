# Approval

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Approval ID | [optional] 
**State** | Pointer to **string** | Approval state | [optional] 
**CompletedAt** | Pointer to **time.Time** | Approval completion timestamp | [optional] 
**Requestor** | Pointer to **string** | Approval requestor | [optional] 
**Context** | Pointer to **string** | Approval context | [optional] 
**CreatedAt** | Pointer to **time.Time** | Approval creation timestamp | [optional] 
**Message** | Pointer to **string** | Approval message | [optional] 
**Tags** | Pointer to **map[string]string** |  | [optional] 
**OnBehalfOf** | Pointer to **string** | If requesting authorization on a user&#39;s behalf, provide the email to let the approvers know. | [optional] 
**Payload** | Pointer to **map[string]interface{}** | Arbitrary JSON data that gets passed to webhooks | [optional] 
**Transactions** | Pointer to [**[]Transaction**](Transaction.md) |  | [optional] 

## Methods

### NewApproval

`func NewApproval() *Approval`

NewApproval instantiates a new Approval object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApprovalWithDefaults

`func NewApprovalWithDefaults() *Approval`

NewApprovalWithDefaults instantiates a new Approval object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Approval) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Approval) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Approval) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *Approval) HasId() bool`

HasId returns a boolean if a field has been set.

### GetState

`func (o *Approval) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *Approval) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *Approval) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *Approval) HasState() bool`

HasState returns a boolean if a field has been set.

### GetCompletedAt

`func (o *Approval) GetCompletedAt() time.Time`

GetCompletedAt returns the CompletedAt field if non-nil, zero value otherwise.

### GetCompletedAtOk

`func (o *Approval) GetCompletedAtOk() (*time.Time, bool)`

GetCompletedAtOk returns a tuple with the CompletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedAt

`func (o *Approval) SetCompletedAt(v time.Time)`

SetCompletedAt sets CompletedAt field to given value.

### HasCompletedAt

`func (o *Approval) HasCompletedAt() bool`

HasCompletedAt returns a boolean if a field has been set.

### GetRequestor

`func (o *Approval) GetRequestor() string`

GetRequestor returns the Requestor field if non-nil, zero value otherwise.

### GetRequestorOk

`func (o *Approval) GetRequestorOk() (*string, bool)`

GetRequestorOk returns a tuple with the Requestor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequestor

`func (o *Approval) SetRequestor(v string)`

SetRequestor sets Requestor field to given value.

### HasRequestor

`func (o *Approval) HasRequestor() bool`

HasRequestor returns a boolean if a field has been set.

### GetContext

`func (o *Approval) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *Approval) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *Approval) SetContext(v string)`

SetContext sets Context field to given value.

### HasContext

`func (o *Approval) HasContext() bool`

HasContext returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Approval) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Approval) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Approval) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Approval) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetMessage

`func (o *Approval) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *Approval) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *Approval) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *Approval) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetTags

`func (o *Approval) GetTags() map[string]string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *Approval) GetTagsOk() (*map[string]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *Approval) SetTags(v map[string]string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *Approval) HasTags() bool`

HasTags returns a boolean if a field has been set.

### GetOnBehalfOf

`func (o *Approval) GetOnBehalfOf() string`

GetOnBehalfOf returns the OnBehalfOf field if non-nil, zero value otherwise.

### GetOnBehalfOfOk

`func (o *Approval) GetOnBehalfOfOk() (*string, bool)`

GetOnBehalfOfOk returns a tuple with the OnBehalfOf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnBehalfOf

`func (o *Approval) SetOnBehalfOf(v string)`

SetOnBehalfOf sets OnBehalfOf field to given value.

### HasOnBehalfOf

`func (o *Approval) HasOnBehalfOf() bool`

HasOnBehalfOf returns a boolean if a field has been set.

### GetPayload

`func (o *Approval) GetPayload() map[string]interface{}`

GetPayload returns the Payload field if non-nil, zero value otherwise.

### GetPayloadOk

`func (o *Approval) GetPayloadOk() (*map[string]interface{}, bool)`

GetPayloadOk returns a tuple with the Payload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayload

`func (o *Approval) SetPayload(v map[string]interface{})`

SetPayload sets Payload field to given value.

### HasPayload

`func (o *Approval) HasPayload() bool`

HasPayload returns a boolean if a field has been set.

### GetTransactions

`func (o *Approval) GetTransactions() []Transaction`

GetTransactions returns the Transactions field if non-nil, zero value otherwise.

### GetTransactionsOk

`func (o *Approval) GetTransactionsOk() (*[]Transaction, bool)`

GetTransactionsOk returns a tuple with the Transactions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactions

`func (o *Approval) SetTransactions(v []Transaction)`

SetTransactions sets Transactions field to given value.

### HasTransactions

`func (o *Approval) HasTransactions() bool`

HasTransactions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


