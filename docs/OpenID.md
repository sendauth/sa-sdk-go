# OpenID

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Issuer** | Pointer to **string** | OpenID Connect issuer URL | [optional] 
**ClientID** | Pointer to **string** | OpenID Connect client ID | [optional] 
**ClientSecret** | Pointer to **string** | OpenID Connect client secret | [optional] 

## Methods

### NewOpenID

`func NewOpenID() *OpenID`

NewOpenID instantiates a new OpenID object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOpenIDWithDefaults

`func NewOpenIDWithDefaults() *OpenID`

NewOpenIDWithDefaults instantiates a new OpenID object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIssuer

`func (o *OpenID) GetIssuer() string`

GetIssuer returns the Issuer field if non-nil, zero value otherwise.

### GetIssuerOk

`func (o *OpenID) GetIssuerOk() (*string, bool)`

GetIssuerOk returns a tuple with the Issuer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuer

`func (o *OpenID) SetIssuer(v string)`

SetIssuer sets Issuer field to given value.

### HasIssuer

`func (o *OpenID) HasIssuer() bool`

HasIssuer returns a boolean if a field has been set.

### GetClientID

`func (o *OpenID) GetClientID() string`

GetClientID returns the ClientID field if non-nil, zero value otherwise.

### GetClientIDOk

`func (o *OpenID) GetClientIDOk() (*string, bool)`

GetClientIDOk returns a tuple with the ClientID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientID

`func (o *OpenID) SetClientID(v string)`

SetClientID sets ClientID field to given value.

### HasClientID

`func (o *OpenID) HasClientID() bool`

HasClientID returns a boolean if a field has been set.

### GetClientSecret

`func (o *OpenID) GetClientSecret() string`

GetClientSecret returns the ClientSecret field if non-nil, zero value otherwise.

### GetClientSecretOk

`func (o *OpenID) GetClientSecretOk() (*string, bool)`

GetClientSecretOk returns a tuple with the ClientSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientSecret

`func (o *OpenID) SetClientSecret(v string)`

SetClientSecret sets ClientSecret field to given value.

### HasClientSecret

`func (o *OpenID) HasClientSecret() bool`

HasClientSecret returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


