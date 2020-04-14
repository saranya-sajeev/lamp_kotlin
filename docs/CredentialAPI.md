# CredentialAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**credentialCreate**](CredentialAPI.md#credentialCreate) | **POST** /type/{type_id}/credential | 
[**credentialDelete**](CredentialAPI.md#credentialDelete) | **DELETE** /type/{type_id}/credential/{access_key} | 
[**credentialList**](CredentialAPI.md#credentialList) | **GET** /type/{type_id}/credential | 
[**credentialUpdate**](CredentialAPI.md#credentialUpdate) | **PUT** /type/{type_id}/credential/{access_key} | 


<a name="credentialCreate"></a>
# **credentialCreate**
> kotlin.Any credentialCreate(typeId, body)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = CredentialAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.credentialCreate(typeId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CredentialAPI#credentialCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CredentialAPI#credentialCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
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

<a name="credentialDelete"></a>
# **credentialDelete**
> kotlin.Any credentialDelete(typeId, accessKey)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = CredentialAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val accessKey : kotlin.String = accessKey_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.credentialDelete(typeId, accessKey)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CredentialAPI#credentialDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CredentialAPI#credentialDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
 **accessKey** | **kotlin.String**|  |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="credentialList"></a>
# **credentialList**
> kotlin.Any credentialList(typeId, transform)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = CredentialAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.credentialList(typeId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CredentialAPI#credentialList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CredentialAPI#credentialList")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
 **transform** | **kotlin.String**|  | [optional]

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="credentialUpdate"></a>
# **credentialUpdate**
> kotlin.Any credentialUpdate(typeId, accessKey, body)



### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = CredentialAPI()
val typeId : kotlin.String = typeId_example // kotlin.String | 
val accessKey : kotlin.String = accessKey_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.credentialUpdate(typeId, accessKey, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CredentialAPI#credentialUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CredentialAPI#credentialUpdate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **typeId** | **kotlin.String**|  |
 **accessKey** | **kotlin.String**|  |
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

