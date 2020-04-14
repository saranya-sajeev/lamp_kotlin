# ActivityEventAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activityEventAllByParticipant**](ActivityEventAPI.md#activityEventAllByParticipant) | **GET** /participant/{participant_id}/activity_event | Get all activity events for a participant.
[**activityEventAllByResearcher**](ActivityEventAPI.md#activityEventAllByResearcher) | **GET** /researcher/{researcher_id}/activity_event | Get all activity events for a researcher by participant.
[**activityEventAllByStudy**](ActivityEventAPI.md#activityEventAllByStudy) | **GET** /study/{study_id}/activity_event | Get all activity events for a study by participant.
[**activityEventCreate**](ActivityEventAPI.md#activityEventCreate) | **POST** /participant/{participant_id}/activity_event | Create a new ActivityEvent for the given Participant.
[**activityEventDelete**](ActivityEventAPI.md#activityEventDelete) | **DELETE** /participant/{participant_id}/activity_event | Delete a ActivityEvent.


<a name="activityEventAllByParticipant"></a>
# **activityEventAllByParticipant**
> kotlin.Array&lt;kotlin.Any&gt; activityEventAllByParticipant(participantId, origin, from, to, transform)

Get all activity events for a participant.

Get the set of all activity events produced by a given participant,  by identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityEventAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val origin : kotlin.String = origin_example // kotlin.String | 
val from : java.sql.Timestamp =  // java.sql.Timestamp | 
val to : java.sql.Timestamp =  // java.sql.Timestamp | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activityEventAllByParticipant(participantId, origin, from, to, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityEventAPI#activityEventAllByParticipant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityEventAPI#activityEventAllByParticipant")
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

<a name="activityEventAllByResearcher"></a>
# **activityEventAllByResearcher**
> kotlin.Array&lt;kotlin.Any&gt; activityEventAllByResearcher(researcherId, origin, from, to, transform)

Get all activity events for a researcher by participant.

Get the set of all activity events produced by participants of any  study conducted by a researcher, by researcher identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityEventAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val origin : kotlin.String = origin_example // kotlin.String | 
val from : java.sql.Timestamp =  // java.sql.Timestamp | 
val to : java.sql.Timestamp =  // java.sql.Timestamp | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activityEventAllByResearcher(researcherId, origin, from, to, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityEventAPI#activityEventAllByResearcher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityEventAPI#activityEventAllByResearcher")
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

<a name="activityEventAllByStudy"></a>
# **activityEventAllByStudy**
> kotlin.Array&lt;kotlin.Any&gt; activityEventAllByStudy(studyId, origin, from, to, transform)

Get all activity events for a study by participant.

Get the set of all activity events produced by participants of a  single study, by study identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityEventAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val origin : kotlin.String = origin_example // kotlin.String | 
val from : java.sql.Timestamp =  // java.sql.Timestamp | 
val to : java.sql.Timestamp =  // java.sql.Timestamp | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activityEventAllByStudy(studyId, origin, from, to, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityEventAPI#activityEventAllByStudy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityEventAPI#activityEventAllByStudy")
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

<a name="activityEventCreate"></a>
# **activityEventCreate**
> kotlin.String activityEventCreate(participantId, activityEvent)

Create a new ActivityEvent for the given Participant.

Create a new ActivityEvent for the given Participant.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityEventAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val activityEvent : ActivityEvent =  // ActivityEvent | 
try {
    val result : kotlin.String = apiInstance.activityEventCreate(participantId, activityEvent)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityEventAPI#activityEventCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityEventAPI#activityEventCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **participantId** | **kotlin.String**|  |
 **activityEvent** | [**ActivityEvent**](ActivityEvent.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="activityEventDelete"></a>
# **activityEventDelete**
> kotlin.String activityEventDelete(participantId, origin, from, to, transform)

Delete a ActivityEvent.

Delete a ActivityEvent.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityEventAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val origin : kotlin.String = origin_example // kotlin.String | 
val from : java.sql.Timestamp =  // java.sql.Timestamp | 
val to : java.sql.Timestamp =  // java.sql.Timestamp | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.activityEventDelete(participantId, origin, from, to, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityEventAPI#activityEventDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityEventAPI#activityEventDelete")
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

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

