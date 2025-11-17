# RoutingRule

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**TagName** | **string** | Name of tag associated with the routing rule | 
**TagValue** | **string** | Tag value that must match for this rule to fire | 
**Description** | Pointer to **string** |  | [optional] 
**TargetType** | **string** | The type of target for the routing rule | 
**TargetId** | **string** | The ID of the target (approval group or user) | 
**TargetEmail** | Pointer to **string** | The email of the target | [optional] 
**TargetName** | Pointer to **string** | The name of the target | [optional] 

## Methods

### NewRoutingRule

`func NewRoutingRule(tagName string, tagValue string, targetType string, targetId string, ) *RoutingRule`

NewRoutingRule instantiates a new RoutingRule object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoutingRuleWithDefaults

`func NewRoutingRuleWithDefaults() *RoutingRule`

NewRoutingRuleWithDefaults instantiates a new RoutingRule object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *RoutingRule) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RoutingRule) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RoutingRule) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *RoutingRule) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTagName

`func (o *RoutingRule) GetTagName() string`

GetTagName returns the TagName field if non-nil, zero value otherwise.

### GetTagNameOk

`func (o *RoutingRule) GetTagNameOk() (*string, bool)`

GetTagNameOk returns a tuple with the TagName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagName

`func (o *RoutingRule) SetTagName(v string)`

SetTagName sets TagName field to given value.


### GetTagValue

`func (o *RoutingRule) GetTagValue() string`

GetTagValue returns the TagValue field if non-nil, zero value otherwise.

### GetTagValueOk

`func (o *RoutingRule) GetTagValueOk() (*string, bool)`

GetTagValueOk returns a tuple with the TagValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTagValue

`func (o *RoutingRule) SetTagValue(v string)`

SetTagValue sets TagValue field to given value.


### GetDescription

`func (o *RoutingRule) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *RoutingRule) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *RoutingRule) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *RoutingRule) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetTargetType

`func (o *RoutingRule) GetTargetType() string`

GetTargetType returns the TargetType field if non-nil, zero value otherwise.

### GetTargetTypeOk

`func (o *RoutingRule) GetTargetTypeOk() (*string, bool)`

GetTargetTypeOk returns a tuple with the TargetType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetType

`func (o *RoutingRule) SetTargetType(v string)`

SetTargetType sets TargetType field to given value.


### GetTargetId

`func (o *RoutingRule) GetTargetId() string`

GetTargetId returns the TargetId field if non-nil, zero value otherwise.

### GetTargetIdOk

`func (o *RoutingRule) GetTargetIdOk() (*string, bool)`

GetTargetIdOk returns a tuple with the TargetId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetId

`func (o *RoutingRule) SetTargetId(v string)`

SetTargetId sets TargetId field to given value.


### GetTargetEmail

`func (o *RoutingRule) GetTargetEmail() string`

GetTargetEmail returns the TargetEmail field if non-nil, zero value otherwise.

### GetTargetEmailOk

`func (o *RoutingRule) GetTargetEmailOk() (*string, bool)`

GetTargetEmailOk returns a tuple with the TargetEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetEmail

`func (o *RoutingRule) SetTargetEmail(v string)`

SetTargetEmail sets TargetEmail field to given value.

### HasTargetEmail

`func (o *RoutingRule) HasTargetEmail() bool`

HasTargetEmail returns a boolean if a field has been set.

### GetTargetName

`func (o *RoutingRule) GetTargetName() string`

GetTargetName returns the TargetName field if non-nil, zero value otherwise.

### GetTargetNameOk

`func (o *RoutingRule) GetTargetNameOk() (*string, bool)`

GetTargetNameOk returns a tuple with the TargetName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetName

`func (o *RoutingRule) SetTargetName(v string)`

SetTargetName sets TargetName field to given value.

### HasTargetName

`func (o *RoutingRule) HasTargetName() bool`

HasTargetName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


