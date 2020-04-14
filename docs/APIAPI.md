# APIAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**aPIQuery**](APIAPI.md#aPIQuery) | **POST** / | Query the LAMP Database.
[**aPISchema**](APIAPI.md#aPISchema) | **GET** / | View the API schema document.


<a name="aPIQuery"></a>
# **aPIQuery**
> kotlin.Any aPIQuery(body)

Query the LAMP Database.

Query the LAMP Database using a transformation document. All GET operations in this API schema document are available by replacing the period with an underscore (i.e. &#x60;$Participant_view(...)&#x60; instead of &#x60;Participant.view(...)&#x60;). The &#x60;origin&#x60;, &#x60;from&#x60;, and &#x60;to&#x60; parameters of EventStream functions are preserved but the &#x60;transform&#x60; parameter is not.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = APIAPI()
val body : kotlin.String = body_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.aPIQuery(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling APIAPI#aPIQuery")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling APIAPI#aPIQuery")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **kotlin.String**|  |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: text/plain, application/json
 - **Accept**: application/json

<a name="aPISchema"></a>
# **aPISchema**
> kotlin.Any aPISchema()

View the API schema document.

View this API schema document from a live server instance.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = APIAPI()
try {
    val result : kotlin.Any = apiInstance.aPISchema()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling APIAPI#aPISchema")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling APIAPI#aPISchema")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

