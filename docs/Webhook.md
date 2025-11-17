# Webhook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | The unique identifier of the webhook | 
**Url** | **string** | The URL where webhook events will be sent | 
**Secret** | Pointer to **string** | Optional secret used to sign webhook payloads (HMAC-SHA256) | [optional] 
**AuthGroupID** | Pointer to **string** | Optional approval group ID to associate with the webhook | [optional] 
**Events** | [**WebhookEvents**](WebhookEvents.md) |  | 
**CreatedAt** | Pointer to **time.Time** | When the webhook was created | [optional] 

## Methods

### NewWebhook

`func NewWebhook(id string, url string, events WebhookEvents, ) *Webhook`

NewWebhook instantiates a new Webhook object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookWithDefaults

`func NewWebhookWithDefaults() *Webhook`

NewWebhookWithDefaults instantiates a new Webhook object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Webhook) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Webhook) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Webhook) SetId(v string)`

SetId sets Id field to given value.


### GetUrl

`func (o *Webhook) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *Webhook) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *Webhook) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetSecret

`func (o *Webhook) GetSecret() string`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *Webhook) GetSecretOk() (*string, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *Webhook) SetSecret(v string)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *Webhook) HasSecret() bool`

HasSecret returns a boolean if a field has been set.

### GetAuthGroupID

`func (o *Webhook) GetAuthGroupID() string`

GetAuthGroupID returns the AuthGroupID field if non-nil, zero value otherwise.

### GetAuthGroupIDOk

`func (o *Webhook) GetAuthGroupIDOk() (*string, bool)`

GetAuthGroupIDOk returns a tuple with the AuthGroupID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthGroupID

`func (o *Webhook) SetAuthGroupID(v string)`

SetAuthGroupID sets AuthGroupID field to given value.

### HasAuthGroupID

`func (o *Webhook) HasAuthGroupID() bool`

HasAuthGroupID returns a boolean if a field has been set.

### GetEvents

`func (o *Webhook) GetEvents() WebhookEvents`

GetEvents returns the Events field if non-nil, zero value otherwise.

### GetEventsOk

`func (o *Webhook) GetEventsOk() (*WebhookEvents, bool)`

GetEventsOk returns a tuple with the Events field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvents

`func (o *Webhook) SetEvents(v WebhookEvents)`

SetEvents sets Events field to given value.


### GetCreatedAt

`func (o *Webhook) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Webhook) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Webhook) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Webhook) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


