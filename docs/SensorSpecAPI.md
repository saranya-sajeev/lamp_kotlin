# SensorSpecAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sensorSpecAll**](SensorSpecAPI.md#sensorSpecAll) | **GET** /sensor_spec | Get all SensorSpecs registered.
[**sensorSpecCreate**](SensorSpecAPI.md#sensorSpecCreate) | **POST** /sensor_spec | Create a new SensorSpec.
[**sensorSpecDelete**](SensorSpecAPI.md#sensorSpecDelete) | **DELETE** /sensor_spec/{sensor_spec_name} | Delete an SensorSpec.
[**sensorSpecUpdate**](SensorSpecAPI.md#sensorSpecUpdate) | **PUT** /sensor_spec/{sensor_spec_name} | Update an SensorSpec.
[**sensorSpecView**](SensorSpecAPI.md#sensorSpecView) | **GET** /sensor_spec/{sensor_spec_name} | Get a SensorSpec.


<a name="sensorSpecAll"></a>
# **sensorSpecAll**
> kotlin.Array&lt;kotlin.Any&gt; sensorSpecAll(transform)

Get all SensorSpecs registered.

Get all SensorSpecs registered by any Researcher.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorSpecAPI()
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorSpecAll(transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorSpecAPI#sensorSpecAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorSpecAPI#sensorSpecAll")
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

<a name="sensorSpecCreate"></a>
# **sensorSpecCreate**
> kotlin.String sensorSpecCreate(sensorSpec)

Create a new SensorSpec.

Create a new SensorSpec.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorSpecAPI()
val sensorSpec : SensorSpec =  // SensorSpec | 
try {
    val result : kotlin.String = apiInstance.sensorSpecCreate(sensorSpec)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorSpecAPI#sensorSpecCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorSpecAPI#sensorSpecCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sensorSpec** | [**SensorSpec**](SensorSpec.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="sensorSpecDelete"></a>
# **sensorSpecDelete**
> kotlin.String sensorSpecDelete(sensorSpecName)

Delete an SensorSpec.

Delete an SensorSpec.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorSpecAPI()
val sensorSpecName : kotlin.String = sensorSpecName_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.sensorSpecDelete(sensorSpecName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorSpecAPI#sensorSpecDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorSpecAPI#sensorSpecDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sensorSpecName** | **kotlin.String**|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="sensorSpecUpdate"></a>
# **sensorSpecUpdate**
> kotlin.String sensorSpecUpdate(sensorSpecName, sensorSpec)

Update an SensorSpec.

Update an SensorSpec.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorSpecAPI()
val sensorSpecName : kotlin.String = sensorSpecName_example // kotlin.String | 
val sensorSpec : SensorSpec =  // SensorSpec | 
try {
    val result : kotlin.String = apiInstance.sensorSpecUpdate(sensorSpecName, sensorSpec)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorSpecAPI#sensorSpecUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorSpecAPI#sensorSpecUpdate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sensorSpecName** | **kotlin.String**|  |
 **sensorSpec** | [**SensorSpec**](SensorSpec.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="sensorSpecView"></a>
# **sensorSpecView**
> kotlin.Array&lt;kotlin.Any&gt; sensorSpecView(sensorSpecName, transform)

Get a SensorSpec.

Get a SensorSpec.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorSpecAPI()
val sensorSpecName : kotlin.String = sensorSpecName_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorSpecView(sensorSpecName, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorSpecAPI#sensorSpecView")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorSpecAPI#sensorSpecView")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sensorSpecName** | **kotlin.String**|  |
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

