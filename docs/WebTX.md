# WebTX

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | Pointer to **string** | Transaction message | [optional] 
**Connectwise** | Pointer to **string** | ConnectWise reference | [optional] 

## Methods

### NewWebTX

`func NewWebTX() *WebTX`

NewWebTX instantiates a new WebTX object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebTXWithDefaults

`func NewWebTXWithDefaults() *WebTX`

NewWebTXWithDefaults instantiates a new WebTX object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *WebTX) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *WebTX) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *WebTX) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *WebTX) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetConnectwise

`func (o *WebTX) GetConnectwise() string`

GetConnectwise returns the Connectwise field if non-nil, zero value otherwise.

### GetConnectwiseOk

`func (o *WebTX) GetConnectwiseOk() (*string, bool)`

GetConnectwiseOk returns a tuple with the Connectwise field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectwise

`func (o *WebTX) SetConnectwise(v string)`

SetConnectwise sets Connectwise field to given value.

### HasConnectwise

`func (o *WebTX) HasConnectwise() bool`

HasConnectwise returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


