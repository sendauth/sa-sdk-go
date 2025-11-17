# WebhookInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** |  | 
**Secret** | Pointer to **string** | Optional secret used to sign webhook payloads (HMAC-SHA256). If a secret is already set, omitting this will preserve the existing secret. | [optional] 
**AuthGroupID** | Pointer to **string** | Optional approval group ID to associate with the webhook | [optional] 
**Events** | [**WebhookEvents**](WebhookEvents.md) |  | 

## Methods

### NewWebhookInput

`func NewWebhookInput(url string, events WebhookEvents, ) *WebhookInput`

NewWebhookInput instantiates a new WebhookInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookInputWithDefaults

`func NewWebhookInputWithDefaults() *WebhookInput`

NewWebhookInputWithDefaults instantiates a new WebhookInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *WebhookInput) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *WebhookInput) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *WebhookInput) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetSecret

`func (o *WebhookInput) GetSecret() string`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *WebhookInput) GetSecretOk() (*string, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *WebhookInput) SetSecret(v string)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *WebhookInput) HasSecret() bool`

HasSecret returns a boolean if a field has been set.

### GetAuthGroupID

`func (o *WebhookInput) GetAuthGroupID() string`

GetAuthGroupID returns the AuthGroupID field if non-nil, zero value otherwise.

### GetAuthGroupIDOk

`func (o *WebhookInput) GetAuthGroupIDOk() (*string, bool)`

GetAuthGroupIDOk returns a tuple with the AuthGroupID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthGroupID

`func (o *WebhookInput) SetAuthGroupID(v string)`

SetAuthGroupID sets AuthGroupID field to given value.

### HasAuthGroupID

`func (o *WebhookInput) HasAuthGroupID() bool`

HasAuthGroupID returns a boolean if a field has been set.

### GetEvents

`func (o *WebhookInput) GetEvents() WebhookEvents`

GetEvents returns the Events field if non-nil, zero value otherwise.

### GetEventsOk

`func (o *WebhookInput) GetEventsOk() (*WebhookEvents, bool)`

GetEventsOk returns a tuple with the Events field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvents

`func (o *WebhookInput) SetEvents(v WebhookEvents)`

SetEvents sets Events field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


