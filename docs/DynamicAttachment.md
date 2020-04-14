
# DynamicAttachment

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **kotlin.String** | The key. |  [optional]
**from** | **kotlin.String** | A globally unique reference for objects. |  [optional]
**to** | **kotlin.String** | Either \&quot;me\&quot; to apply to the attachment owner only, the ID of an object owned  by the attachment owner, or a string representing the child object type to apply to. |  [optional]
**triggers** | [**kotlin.Array&lt;kotlin.Any&gt;**](kotlin.Any.md) | The API triggers that activate script execution. These will be event stream types  or object types in the API, or, if scheduling execution periodically, a cron-job string  prefixed with \&quot;!\&quot; (exclamation point). |  [optional]
**language** | **kotlin.String** | The script language. |  [optional]
**contents** | **kotlin.String** | The script contents. |  [optional]
**requirements** | [**kotlin.Array&lt;kotlin.Any&gt;**](kotlin.Any.md) | The script requirements. |  [optional]



