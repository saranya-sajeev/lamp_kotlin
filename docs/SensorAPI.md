# SensorAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sensorAll**](SensorAPI.md#sensorAll) | **GET** /sensor | Get the set of all sensors.
[**sensorAllByParticipant**](SensorAPI.md#sensorAllByParticipant) | **GET** /participant/{participant_id}/sensor | Get all sensors for a participant.
[**sensorAllByResearcher**](SensorAPI.md#sensorAllByResearcher) | **GET** /researcher/{researcher_id}/sensor | Get all sensors for a researcher.
[**sensorAllByStudy**](SensorAPI.md#sensorAllByStudy) | **GET** /study/{study_id}/sensor | View all sensors in a study.
[**sensorCreate**](SensorAPI.md#sensorCreate) | **POST** /study/{study_id}/sensor | Create a new Sensor under the given Study.
[**sensorDelete**](SensorAPI.md#sensorDelete) | **DELETE** /sensor/{sensor_id} | Delete a Sensor.
[**sensorUpdate**](SensorAPI.md#sensorUpdate) | **PUT** /sensor/{sensor_id} | Update an Sensor&#39;s settings.
[**sensorView**](SensorAPI.md#sensorView) | **GET** /sensor/{sensor_id} | Get a single sensor, by identifier.


<a name="sensorAll"></a>
# **sensorAll**
> kotlin.Array&lt;kotlin.Any&gt; sensorAll(transform)

Get the set of all sensors.

Get the set of all sensors.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorAPI()
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorAll(transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorAPI#sensorAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorAPI#sensorAll")
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

<a name="sensorAllByParticipant"></a>
# **sensorAllByParticipant**
> kotlin.Array&lt;kotlin.Any&gt; sensorAllByParticipant(participantId, transform)

Get all sensors for a participant.

Get the set of all sensors available to a participant, by participant  identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorAllByParticipant(participantId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorAPI#sensorAllByParticipant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorAPI#sensorAllByParticipant")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **participantId** | **kotlin.String**|  |
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

<a name="sensorAllByResearcher"></a>
# **sensorAllByResearcher**
> kotlin.Array&lt;kotlin.Any&gt; sensorAllByResearcher(researcherId, transform)

Get all sensors for a researcher.

Get the set of all sensors available to participants of any study conducted  by a researcher, by researcher identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorAllByResearcher(researcherId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorAPI#sensorAllByResearcher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorAPI#sensorAllByResearcher")
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

<a name="sensorAllByStudy"></a>
# **sensorAllByStudy**
> kotlin.Array&lt;kotlin.Any&gt; sensorAllByStudy(studyId, transform)

View all sensors in a study.

Get the set of all sensors available to participants of a single  study, by study identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorAllByStudy(studyId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorAPI#sensorAllByStudy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorAPI#sensorAllByStudy")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **studyId** | **kotlin.String**|  |
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

<a name="sensorCreate"></a>
# **sensorCreate**
> kotlin.String sensorCreate(studyId, sensor)

Create a new Sensor under the given Study.

Create a new Sensor under the given Study.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val sensor : Sensor =  // Sensor | 
try {
    val result : kotlin.String = apiInstance.sensorCreate(studyId, sensor)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorAPI#sensorCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorAPI#sensorCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **studyId** | **kotlin.String**|  |
 **sensor** | [**Sensor**](Sensor.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="sensorDelete"></a>
# **sensorDelete**
> kotlin.String sensorDelete(sensorId)

Delete a Sensor.

Delete a Sensor.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorAPI()
val sensorId : kotlin.String = sensorId_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.sensorDelete(sensorId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorAPI#sensorDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorAPI#sensorDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sensorId** | **kotlin.String**|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="sensorUpdate"></a>
# **sensorUpdate**
> kotlin.String sensorUpdate(sensorId, sensor)

Update an Sensor&#39;s settings.

Update an Sensor&#39;s settings.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorAPI()
val sensorId : kotlin.String = sensorId_example // kotlin.String | 
val sensor : Sensor =  // Sensor | 
try {
    val result : kotlin.String = apiInstance.sensorUpdate(sensorId, sensor)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorAPI#sensorUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorAPI#sensorUpdate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sensorId** | **kotlin.String**|  |
 **sensor** | [**Sensor**](Sensor.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="sensorView"></a>
# **sensorView**
> kotlin.Array&lt;kotlin.Any&gt; sensorView(sensorId, transform)

Get a single sensor, by identifier.

Get a single sensor, by identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorAPI()
val sensorId : kotlin.String = sensorId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorView(sensorId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorAPI#sensorView")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorAPI#sensorView")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sensorId** | **kotlin.String**|  |
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

