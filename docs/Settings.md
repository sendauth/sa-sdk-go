# Settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Subdomain** | Pointer to **string** | Organization subdomain | [optional] 
**Name** | Pointer to **string** | Organization name | [optional] 
**OpenID** | Pointer to [**OpenID**](OpenID.md) |  | [optional] 
**ScimSecret** | Pointer to **string** | SCIM API secret | [optional] 
**EmailTemplate** | Pointer to **string** | Email notification template | [optional] 
**SmsTemplate** | Pointer to **string** | SMS notification template | [optional] 
**ConnectWise** | Pointer to [**ConnectWise**](ConnectWise.md) |  | [optional] 

## Methods

### NewSettings

`func NewSettings() *Settings`

NewSettings instantiates a new Settings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSettingsWithDefaults

`func NewSettingsWithDefaults() *Settings`

NewSettingsWithDefaults instantiates a new Settings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSubdomain

`func (o *Settings) GetSubdomain() string`

GetSubdomain returns the Subdomain field if non-nil, zero value otherwise.

### GetSubdomainOk

`func (o *Settings) GetSubdomainOk() (*string, bool)`

GetSubdomainOk returns a tuple with the Subdomain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubdomain

`func (o *Settings) SetSubdomain(v string)`

SetSubdomain sets Subdomain field to given value.

### HasSubdomain

`func (o *Settings) HasSubdomain() bool`

HasSubdomain returns a boolean if a field has been set.

### GetName

`func (o *Settings) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Settings) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Settings) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Settings) HasName() bool`

HasName returns a boolean if a field has been set.

### GetOpenID

`func (o *Settings) GetOpenID() OpenID`

GetOpenID returns the OpenID field if non-nil, zero value otherwise.

### GetOpenIDOk

`func (o *Settings) GetOpenIDOk() (*OpenID, bool)`

GetOpenIDOk returns a tuple with the OpenID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenID

`func (o *Settings) SetOpenID(v OpenID)`

SetOpenID sets OpenID field to given value.

### HasOpenID

`func (o *Settings) HasOpenID() bool`

HasOpenID returns a boolean if a field has been set.

### GetScimSecret

`func (o *Settings) GetScimSecret() string`

GetScimSecret returns the ScimSecret field if non-nil, zero value otherwise.

### GetScimSecretOk

`func (o *Settings) GetScimSecretOk() (*string, bool)`

GetScimSecretOk returns a tuple with the ScimSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScimSecret

`func (o *Settings) SetScimSecret(v string)`

SetScimSecret sets ScimSecret field to given value.

### HasScimSecret

`func (o *Settings) HasScimSecret() bool`

HasScimSecret returns a boolean if a field has been set.

### GetEmailTemplate

`func (o *Settings) GetEmailTemplate() string`

GetEmailTemplate returns the EmailTemplate field if non-nil, zero value otherwise.

### GetEmailTemplateOk

`func (o *Settings) GetEmailTemplateOk() (*string, bool)`

GetEmailTemplateOk returns a tuple with the EmailTemplate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailTemplate

`func (o *Settings) SetEmailTemplate(v string)`

SetEmailTemplate sets EmailTemplate field to given value.

### HasEmailTemplate

`func (o *Settings) HasEmailTemplate() bool`

HasEmailTemplate returns a boolean if a field has been set.

### GetSmsTemplate

`func (o *Settings) GetSmsTemplate() string`

GetSmsTemplate returns the SmsTemplate field if non-nil, zero value otherwise.

### GetSmsTemplateOk

`func (o *Settings) GetSmsTemplateOk() (*string, bool)`

GetSmsTemplateOk returns a tuple with the SmsTemplate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSmsTemplate

`func (o *Settings) SetSmsTemplate(v string)`

SetSmsTemplate sets SmsTemplate field to given value.

### HasSmsTemplate

`func (o *Settings) HasSmsTemplate() bool`

HasSmsTemplate returns a boolean if a field has been set.

### GetConnectWise

`func (o *Settings) GetConnectWise() ConnectWise`

GetConnectWise returns the ConnectWise field if non-nil, zero value otherwise.

### GetConnectWiseOk

`func (o *Settings) GetConnectWiseOk() (*ConnectWise, bool)`

GetConnectWiseOk returns a tuple with the ConnectWise field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectWise

`func (o *Settings) SetConnectWise(v ConnectWise)`

SetConnectWise sets ConnectWise field to given value.

### HasConnectWise

`func (o *Settings) HasConnectWise() bool`

HasConnectWise returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


