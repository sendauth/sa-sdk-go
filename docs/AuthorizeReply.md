# AuthorizeReply

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TxID** | Pointer to **string** | Transaction ID for the transaction that&#39;s been sent to a user | [optional] 
**ApprovalID** | Pointer to **string** | Approval ID for the approval that&#39;s been sent to an approval group | [optional] 

## Methods

### NewAuthorizeReply

`func NewAuthorizeReply() *AuthorizeReply`

NewAuthorizeReply instantiates a new AuthorizeReply object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthorizeReplyWithDefaults

`func NewAuthorizeReplyWithDefaults() *AuthorizeReply`

NewAuthorizeReplyWithDefaults instantiates a new AuthorizeReply object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTxID

`func (o *AuthorizeReply) GetTxID() string`

GetTxID returns the TxID field if non-nil, zero value otherwise.

### GetTxIDOk

`func (o *AuthorizeReply) GetTxIDOk() (*string, bool)`

GetTxIDOk returns a tuple with the TxID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTxID

`func (o *AuthorizeReply) SetTxID(v string)`

SetTxID sets TxID field to given value.

### HasTxID

`func (o *AuthorizeReply) HasTxID() bool`

HasTxID returns a boolean if a field has been set.

### GetApprovalID

`func (o *AuthorizeReply) GetApprovalID() string`

GetApprovalID returns the ApprovalID field if non-nil, zero value otherwise.

### GetApprovalIDOk

`func (o *AuthorizeReply) GetApprovalIDOk() (*string, bool)`

GetApprovalIDOk returns a tuple with the ApprovalID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApprovalID

`func (o *AuthorizeReply) SetApprovalID(v string)`

SetApprovalID sets ApprovalID field to given value.

### HasApprovalID

`func (o *AuthorizeReply) HasApprovalID() bool`

HasApprovalID returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


