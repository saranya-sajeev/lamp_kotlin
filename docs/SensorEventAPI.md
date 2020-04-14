# SensorEventAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sensorEventAllByParticipant**](SensorEventAPI.md#sensorEventAllByParticipant) | **GET** /participant/{participant_id}/sensor_event | Get all sensor events for a participant.
[**sensorEventAllByResearcher**](SensorEventAPI.md#sensorEventAllByResearcher) | **GET** /researcher/{researcher_id}/sensor_event | Get all sensor events for a researcher by participant.
[**sensorEventAllByStudy**](SensorEventAPI.md#sensorEventAllByStudy) | **GET** /study/{study_id}/sensor_event | Get all sensor events for a study by participant.
[**sensorEventCreate**](SensorEventAPI.md#sensorEventCreate) | **POST** /participant/{participant_id}/sensor_event | Create a new SensorEvent for the given Participant.
[**sensorEventDelete**](SensorEventAPI.md#sensorEventDelete) | **DELETE** /participant/{participant_id}/sensor_event | Delete a sensor event.


<a name="sensorEventAllByParticipant"></a>
# **sensorEventAllByParticipant**
> kotlin.Array&lt;kotlin.Any&gt; sensorEventAllByParticipant(participantId, origin, from, to, transform)

Get all sensor events for a participant.

Get the set of all sensor events produced by the given participant.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorEventAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val origin : kotlin.String = origin_example // kotlin.String | 
val from : java.sql.Timestamp =  // java.sql.Timestamp | 
val to : java.sql.Timestamp =  // java.sql.Timestamp | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorEventAllByParticipant(participantId, origin, from, to, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorEventAPI#sensorEventAllByParticipant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorEventAPI#sensorEventAllByParticipant")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **participantId** | **kotlin.String**|  |
 **origin** | **kotlin.String**|  | [optional]
 **from** | [**java.sql.Timestamp**](.md)|  | [optional]
 **to** | [**java.sql.Timestamp**](.md)|  | [optional]
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

<a name="sensorEventAllByResearcher"></a>
# **sensorEventAllByResearcher**
> kotlin.Array&lt;kotlin.Any&gt; sensorEventAllByResearcher(researcherId, origin, from, to, transform)

Get all sensor events for a researcher by participant.

Get the set of all sensor events produced by participants of any  study conducted by a researcher, by researcher identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorEventAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val origin : kotlin.String = origin_example // kotlin.String | 
val from : java.sql.Timestamp =  // java.sql.Timestamp | 
val to : java.sql.Timestamp =  // java.sql.Timestamp | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorEventAllByResearcher(researcherId, origin, from, to, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorEventAPI#sensorEventAllByResearcher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorEventAPI#sensorEventAllByResearcher")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **researcherId** | **kotlin.String**|  |
 **origin** | **kotlin.String**|  | [optional]
 **from** | [**java.sql.Timestamp**](.md)|  | [optional]
 **to** | [**java.sql.Timestamp**](.md)|  | [optional]
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

<a name="sensorEventAllByStudy"></a>
# **sensorEventAllByStudy**
> kotlin.Array&lt;kotlin.Any&gt; sensorEventAllByStudy(studyId, origin, from, to, transform)

Get all sensor events for a study by participant.

Get the set of all sensor events produced by participants of a  single study, by study identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorEventAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val origin : kotlin.String = origin_example // kotlin.String | 
val from : java.sql.Timestamp =  // java.sql.Timestamp | 
val to : java.sql.Timestamp =  // java.sql.Timestamp | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.sensorEventAllByStudy(studyId, origin, from, to, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorEventAPI#sensorEventAllByStudy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorEventAPI#sensorEventAllByStudy")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **studyId** | **kotlin.String**|  |
 **origin** | **kotlin.String**|  | [optional]
 **from** | [**java.sql.Timestamp**](.md)|  | [optional]
 **to** | [**java.sql.Timestamp**](.md)|  | [optional]
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

<a name="sensorEventCreate"></a>
# **sensorEventCreate**
> kotlin.String sensorEventCreate(participantId, sensorEvent)

Create a new SensorEvent for the given Participant.

Create a new SensorEvent for the given Participant.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorEventAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val sensorEvent : SensorEvent =  // SensorEvent | 
try {
    val result : kotlin.String = apiInstance.sensorEventCreate(participantId, sensorEvent)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorEventAPI#sensorEventCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorEventAPI#sensorEventCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **participantId** | **kotlin.String**|  |
 **sensorEvent** | [**SensorEvent**](SensorEvent.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="sensorEventDelete"></a>
# **sensorEventDelete**
> kotlin.String sensorEventDelete(participantId, origin, from, to)

Delete a sensor event.

Delete a sensor event.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = SensorEventAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val origin : kotlin.String = origin_example // kotlin.String | 
val from : java.sql.Timestamp =  // java.sql.Timestamp | 
val to : java.sql.Timestamp =  // java.sql.Timestamp | 
try {
    val result : kotlin.String = apiInstance.sensorEventDelete(participantId, origin, from, to)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SensorEventAPI#sensorEventDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SensorEventAPI#sensorEventDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **participantId** | **kotlin.String**|  |
 **origin** | **kotlin.String**|  | [optional]
 **from** | [**java.sql.Timestamp**](.md)|  | [optional]
 **to** | [**java.sql.Timestamp**](.md)|  | [optional]

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

