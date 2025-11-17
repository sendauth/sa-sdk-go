# WebhookEvents

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Verify** | Pointer to **bool** | When true, transaction verifications will invoke the webhook | [optional] 
**Deny** | Pointer to **bool** | When true, transaction denials will invoke the webhook | [optional] 

## Methods

### NewWebhookEvents

`func NewWebhookEvents() *WebhookEvents`

NewWebhookEvents instantiates a new WebhookEvents object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookEventsWithDefaults

`func NewWebhookEventsWithDefaults() *WebhookEvents`

NewWebhookEventsWithDefaults instantiates a new WebhookEvents object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVerify

`func (o *WebhookEvents) GetVerify() bool`

GetVerify returns the Verify field if non-nil, zero value otherwise.

### GetVerifyOk

`func (o *WebhookEvents) GetVerifyOk() (*bool, bool)`

GetVerifyOk returns a tuple with the Verify field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerify

`func (o *WebhookEvents) SetVerify(v bool)`

SetVerify sets Verify field to given value.

### HasVerify

`func (o *WebhookEvents) HasVerify() bool`

HasVerify returns a boolean if a field has been set.

### GetDeny

`func (o *WebhookEvents) GetDeny() bool`

GetDeny returns the Deny field if non-nil, zero value otherwise.

### GetDenyOk

`func (o *WebhookEvents) GetDenyOk() (*bool, bool)`

GetDenyOk returns a tuple with the Deny field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeny

`func (o *WebhookEvents) SetDeny(v bool)`

SetDeny sets Deny field to given value.

### HasDeny

`func (o *WebhookEvents) HasDeny() bool`

HasDeny returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


