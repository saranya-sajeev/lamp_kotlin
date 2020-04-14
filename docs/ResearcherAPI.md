# ResearcherAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**researcherAll**](ResearcherAPI.md#researcherAll) | **GET** /researcher | Get the set of all researchers.
[**researcherCreate**](ResearcherAPI.md#researcherCreate) | **POST** /researcher | Create a new Researcher.
[**researcherDelete**](ResearcherAPI.md#researcherDelete) | **DELETE** /researcher/{researcher_id} | Delete a researcher.
[**researcherUpdate**](ResearcherAPI.md#researcherUpdate) | **PUT** /researcher/{researcher_id} | Update a Researcher&#39;s settings.
[**researcherView**](ResearcherAPI.md#researcherView) | **GET** /researcher/{researcher_id} | Get a single researcher, by identifier.


<a name="researcherAll"></a>
# **researcherAll**
> kotlin.Array&lt;kotlin.Any&gt; researcherAll(transform)

Get the set of all researchers.

Get the set of all researchers.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ResearcherAPI()
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.researcherAll(transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResearcherAPI#researcherAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResearcherAPI#researcherAll")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transform** | **kotlin.String**|  | [optional]

### Return type

[**kotlin.Array&lt;kotlin.Any&gt;**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="researcherCreate"></a>
# **researcherCreate**
> kotlin.String researcherCreate(researcher)

Create a new Researcher.

Create a new Researcher.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ResearcherAPI()
val researcher : Researcher =  // Researcher | 
try {
    val result : kotlin.String = apiInstance.researcherCreate(researcher)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResearcherAPI#researcherCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResearcherAPI#researcherCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **researcher** | [**Researcher**](Researcher.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="researcherDelete"></a>
# **researcherDelete**
> kotlin.String researcherDelete(researcherId)

Delete a researcher.

Delete a researcher.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ResearcherAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.researcherDelete(researcherId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResearcherAPI#researcherDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResearcherAPI#researcherDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **researcherId** | **kotlin.String**|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="researcherUpdate"></a>
# **researcherUpdate**
> kotlin.String researcherUpdate(researcherId, researcher, transform)

Update a Researcher&#39;s settings.

Update a Researcher&#39;s settings.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ResearcherAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val researcher : Researcher =  // Researcher | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.researcherUpdate(researcherId, researcher, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResearcherAPI#researcherUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResearcherAPI#researcherUpdate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **researcherId** | **kotlin.String**|  |
 **researcher** | [**Researcher**](Researcher.md)|  |
 **transform** | **kotlin.String**|  | [optional]

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="researcherView"></a>
# **researcherView**
> kotlin.Array&lt;kotlin.Any&gt; researcherView(researcherId, transform)

Get a single researcher, by identifier.

Get a single researcher, by identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ResearcherAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.researcherView(researcherId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResearcherAPI#researcherView")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResearcherAPI#researcherView")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **researcherId** | **kotlin.String**|  |
 **transform** | **kotlin.String**|  | [optional]

### Return type

[**kotlin.Array&lt;kotlin.Any&gt;**](kotlin.Any.md)

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

