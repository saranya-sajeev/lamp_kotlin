# TypeAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**typeGetAttachment**](TypeAPI.md#typeGetAttachment) | **GET** /type/{type_id}/attachment/{attachment_key} | 
[**typeGetDynamicAttachment**](TypeAPI.md#typeGetDynamicAttachment) | **GET** /type/{type_id}/attachment/dynamic/{attachment_key} | 
[**typeListAttachments**](TypeAPI.md#typeListAttachments) | **GET** /type/{type_id}/attachment | 
[**typeParent**](TypeAPI.md#typeParent) | **GET** /type/{type_id}/parent | Find the owner(s) of the resource.
[**typeSetAttachment**](TypeAPI.md#typeSetAttachment) | **PUT** /type/{type_id}/attachment/{attachment_key}/{target} | 
[**typeSetDynamicAttachment**](TypeAPI.md#typeSetDynamicAttachment) | **PUT** /type/{type_id}/attachment/dynamic/{attachment_key}/{target} | 


<a name="typeGetAttachment"></a>
# **typeGetAttachment**
> kotlin.Any typeGetAttachment(typeId, attachmentKey)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = TypeAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val attachmentKey : kotlin.String = attachmentKey_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.typeGetAttachment(typeId, attachmentKey)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TypeAPI#typeGetAttachment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TypeAPI#typeGetAttachment")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
 **attachmentKey** | **kotlin.String**|  |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="typeGetDynamicAttachment"></a>
# **typeGetDynamicAttachment**
> kotlin.Any typeGetDynamicAttachment(typeId, attachmentKey, invokeAlways, includeLogs, ignoreOutput)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = TypeAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val attachmentKey : kotlin.String = attachmentKey_example // kotlin.String | 
val invokeAlways : kotlin.Boolean = true // kotlin.Boolean | 
val includeLogs : kotlin.Boolean = true // kotlin.Boolean | 
val ignoreOutput : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : kotlin.Any = apiInstance.typeGetDynamicAttachment(typeId, attachmentKey, invokeAlways, includeLogs, ignoreOutput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TypeAPI#typeGetDynamicAttachment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TypeAPI#typeGetDynamicAttachment")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
 **attachmentKey** | **kotlin.String**|  |
 **invokeAlways** | **kotlin.Boolean**|  |
 **includeLogs** | **kotlin.Boolean**|  |
 **ignoreOutput** | **kotlin.Boolean**|  |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="typeListAttachments"></a>
# **typeListAttachments**
> kotlin.Any typeListAttachments(typeId)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = TypeAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.typeListAttachments(typeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TypeAPI#typeListAttachments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TypeAPI#typeListAttachments")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="typeParent"></a>
# **typeParent**
> kotlin.String typeParent(typeId, transform)

Find the owner(s) of the resource.

Get the parent type identifier of the data structure referenced by the identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = TypeAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.typeParent(typeId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TypeAPI#typeParent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TypeAPI#typeParent")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
 **transform** | **kotlin.String**|  | [optional]

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="typeSetAttachment"></a>
# **typeSetAttachment**
> kotlin.Any typeSetAttachment(typeId, target, attachmentKey, body)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = TypeAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val target : kotlin.String = target_example // kotlin.String | 
val attachmentKey : kotlin.String = attachmentKey_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.typeSetAttachment(typeId, target, attachmentKey, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TypeAPI#typeSetAttachment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TypeAPI#typeSetAttachment")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
 **target** | **kotlin.String**|  |
 **attachmentKey** | **kotlin.String**|  |
 **body** | **kotlin.Any**|  |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="typeSetDynamicAttachment"></a>
# **typeSetDynamicAttachment**
> kotlin.Any typeSetDynamicAttachment(typeId, target, attachmentKey, invokeOnce, dynamicAttachment)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = TypeAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val target : kotlin.String = target_example // kotlin.String | 
val attachmentKey : kotlin.String = attachmentKey_example // kotlin.String | 
val invokeOnce : kotlin.Boolean = true // kotlin.Boolean | 
val dynamicAttachment : DynamicAttachment =  // DynamicAttachment | 
try {
    val result : kotlin.Any = apiInstance.typeSetDynamicAttachment(typeId, target, attachmentKey, invokeOnce, dynamicAttachment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TypeAPI#typeSetDynamicAttachment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TypeAPI#typeSetDynamicAttachment")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
 **target** | **kotlin.String**|  |
 **attachmentKey** | **kotlin.String**|  |
 **invokeOnce** | **kotlin.Boolean**|  |
 **dynamicAttachment** | [**DynamicAttachment**](DynamicAttachment.md)|  |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

