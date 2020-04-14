# ActivitySpecAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activitySpecAll**](ActivitySpecAPI.md#activitySpecAll) | **GET** /activity_spec | Get all ActivitySpecs registered.
[**activitySpecCreate**](ActivitySpecAPI.md#activitySpecCreate) | **POST** /activity_spec | Create a new ActivitySpec.
[**activitySpecDelete**](ActivitySpecAPI.md#activitySpecDelete) | **DELETE** /activity_spec/{activity_spec_name} | Delete an ActivitySpec.
[**activitySpecUpdate**](ActivitySpecAPI.md#activitySpecUpdate) | **PUT** /activity_spec/{activity_spec_name} | Update an ActivitySpec.
[**activitySpecView**](ActivitySpecAPI.md#activitySpecView) | **GET** /activity_spec/{activity_spec_name} | View an ActivitySpec.


<a name="activitySpecAll"></a>
# **activitySpecAll**
> kotlin.Array&lt;kotlin.Any&gt; activitySpecAll(transform)

Get all ActivitySpecs registered.

Get all ActivitySpecs registered.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivitySpecAPI()
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activitySpecAll(transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivitySpecAPI#activitySpecAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivitySpecAPI#activitySpecAll")
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

<a name="activitySpecCreate"></a>
# **activitySpecCreate**
> kotlin.String activitySpecCreate(activitySpec)

Create a new ActivitySpec.

Create a new ActivitySpec.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivitySpecAPI()
val activitySpec : ActivitySpec =  // ActivitySpec | 
try {
    val result : kotlin.String = apiInstance.activitySpecCreate(activitySpec)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivitySpecAPI#activitySpecCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivitySpecAPI#activitySpecCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activitySpec** | [**ActivitySpec**](ActivitySpec.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="activitySpecDelete"></a>
# **activitySpecDelete**
> kotlin.String activitySpecDelete(activitySpecName)

Delete an ActivitySpec.

Delete an ActivitySpec.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivitySpecAPI()
val activitySpecName : kotlin.String = activitySpecName_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.activitySpecDelete(activitySpecName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivitySpecAPI#activitySpecDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivitySpecAPI#activitySpecDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activitySpecName** | **kotlin.String**|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="activitySpecUpdate"></a>
# **activitySpecUpdate**
> kotlin.String activitySpecUpdate(activitySpecName, activitySpec)

Update an ActivitySpec.

Update an ActivitySpec.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivitySpecAPI()
val activitySpecName : kotlin.String = activitySpecName_example // kotlin.String | 
val activitySpec : ActivitySpec =  // ActivitySpec | 
try {
    val result : kotlin.String = apiInstance.activitySpecUpdate(activitySpecName, activitySpec)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivitySpecAPI#activitySpecUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivitySpecAPI#activitySpecUpdate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activitySpecName** | **kotlin.String**|  |
 **activitySpec** | [**ActivitySpec**](ActivitySpec.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="activitySpecView"></a>
# **activitySpecView**
> kotlin.String activitySpecView(activitySpecName, transform)

View an ActivitySpec.

View an ActivitySpec.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivitySpecAPI()
val activitySpecName : kotlin.String = activitySpecName_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.activitySpecView(activitySpecName, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivitySpecAPI#activitySpecView")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivitySpecAPI#activitySpecView")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activitySpecName** | **kotlin.String**|  |
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

