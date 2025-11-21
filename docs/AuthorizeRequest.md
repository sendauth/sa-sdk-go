# AuthorizeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | **string** |  | 
**Tag** | **map[string]string** |  | 
**OnBehalfOf** | Pointer to **string** | If requesting authorization on a user&#39;s behalf, provide the email to let the approvers know. | [optional] 
**Context** | Pointer to **string** |  | [optional] 
**Payload** | Pointer to **map[string]interface{}** | Arbitrary JSON data that gets passed to webhooks | [optional] 

## Methods

### NewAuthorizeRequest

`func NewAuthorizeRequest(message string, tag map[string]string, ) *AuthorizeRequest`

NewAuthorizeRequest instantiates a new AuthorizeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuthorizeRequestWithDefaults

`func NewAuthorizeRequestWithDefaults() *AuthorizeRequest`

NewAuthorizeRequestWithDefaults instantiates a new AuthorizeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *AuthorizeRequest) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *AuthorizeRequest) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *AuthorizeRequest) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetTag

`func (o *AuthorizeRequest) GetTag() map[string]string`

GetTag returns the Tag field if non-nil, zero value otherwise.

### GetTagOk

`func (o *AuthorizeRequest) GetTagOk() (*map[string]string, bool)`

GetTagOk returns a tuple with the Tag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTag

`func (o *AuthorizeRequest) SetTag(v map[string]string)`

SetTag sets Tag field to given value.


### GetOnBehalfOf

`func (o *AuthorizeRequest) GetOnBehalfOf() string`

GetOnBehalfOf returns the OnBehalfOf field if non-nil, zero value otherwise.

### GetOnBehalfOfOk

`func (o *AuthorizeRequest) GetOnBehalfOfOk() (*string, bool)`

GetOnBehalfOfOk returns a tuple with the OnBehalfOf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnBehalfOf

`func (o *AuthorizeRequest) SetOnBehalfOf(v string)`

SetOnBehalfOf sets OnBehalfOf field to given value.

### HasOnBehalfOf

`func (o *AuthorizeRequest) HasOnBehalfOf() bool`

HasOnBehalfOf returns a boolean if a field has been set.

### GetContext

`func (o *AuthorizeRequest) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *AuthorizeRequest) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *AuthorizeRequest) SetContext(v string)`

SetContext sets Context field to given value.

### HasContext

`func (o *AuthorizeRequest) HasContext() bool`

HasContext returns a boolean if a field has been set.

### GetPayload

`func (o *AuthorizeRequest) GetPayload() map[string]interface{}`

GetPayload returns the Payload field if non-nil, zero value otherwise.

### GetPayloadOk

`func (o *AuthorizeRequest) GetPayloadOk() (*map[string]interface{}, bool)`

GetPayloadOk returns a tuple with the Payload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayload

`func (o *AuthorizeRequest) SetPayload(v map[string]interface{})`

SetPayload sets Payload field to given value.

### HasPayload

`func (o *AuthorizeRequest) HasPayload() bool`

HasPayload returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


