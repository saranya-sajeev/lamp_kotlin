# ParticipantAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**participantAll**](ParticipantAPI.md#participantAll) | **GET** /participant | Get the set of all participants.
[**participantAllByResearcher**](ParticipantAPI.md#participantAllByResearcher) | **GET** /researcher/{researcher_id}/participant | Get the set of all participants under a single researcher.
[**participantAllByStudy**](ParticipantAPI.md#participantAllByStudy) | **GET** /study/{study_id}/participant | Get the set of all participants in a single study.
[**participantCreate**](ParticipantAPI.md#participantCreate) | **POST** /study/{study_id}/participant | Create a new Participant for the given Study.
[**participantDelete**](ParticipantAPI.md#participantDelete) | **DELETE** /participant/{participant_id} | Delete a participant AND all owned data or event streams.
[**participantUpdate**](ParticipantAPI.md#participantUpdate) | **PUT** /participant/{participant_id} | Update a Participant&#39;s settings.
[**participantView**](ParticipantAPI.md#participantView) | **GET** /participant/{participant_id} | Get a single participant, by identifier.


<a name="participantAll"></a>
# **participantAll**
> kotlin.Array&lt;kotlin.Any&gt; participantAll(transform)

Get the set of all participants.

Get the set of all participants.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ParticipantAPI()
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.participantAll(transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipantAPI#participantAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipantAPI#participantAll")
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

<a name="participantAllByResearcher"></a>
# **participantAllByResearcher**
> kotlin.Array&lt;kotlin.Any&gt; participantAllByResearcher(researcherId, transform)

Get the set of all participants under a single researcher.

Get the set of all participants under a single researcher.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ParticipantAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.participantAllByResearcher(researcherId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipantAPI#participantAllByResearcher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipantAPI#participantAllByResearcher")
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

<a name="participantAllByStudy"></a>
# **participantAllByStudy**
> kotlin.Array&lt;kotlin.Any&gt; participantAllByStudy(studyId, transform)

Get the set of all participants in a single study.

Get the set of all participants in a single study.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ParticipantAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.participantAllByStudy(studyId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipantAPI#participantAllByStudy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipantAPI#participantAllByStudy")
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

<a name="participantCreate"></a>
# **participantCreate**
> kotlin.String participantCreate(studyId, participant)

Create a new Participant for the given Study.

Create a new Participant for the given Study.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ParticipantAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val participant : Participant =  // Participant | 
try {
    val result : kotlin.String = apiInstance.participantCreate(studyId, participant)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipantAPI#participantCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipantAPI#participantCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **studyId** | **kotlin.String**|  |
 **participant** | [**Participant**](Participant.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="participantDelete"></a>
# **participantDelete**
> kotlin.String participantDelete(participantId)

Delete a participant AND all owned data or event streams.

Delete a participant AND all owned data or event streams.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ParticipantAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.participantDelete(participantId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipantAPI#participantDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipantAPI#participantDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **participantId** | **kotlin.String**|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="participantUpdate"></a>
# **participantUpdate**
> kotlin.String participantUpdate(participantId, participant)

Update a Participant&#39;s settings.

Update a Participant&#39;s settings.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ParticipantAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val participant : Participant =  // Participant | 
try {
    val result : kotlin.String = apiInstance.participantUpdate(participantId, participant)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipantAPI#participantUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipantAPI#participantUpdate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **participantId** | **kotlin.String**|  |
 **participant** | [**Participant**](Participant.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="participantView"></a>
# **participantView**
> kotlin.Array&lt;kotlin.Any&gt; participantView(participantId, transform)

Get a single participant, by identifier.

Get a single participant, by identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ParticipantAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.participantView(participantId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipantAPI#participantView")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipantAPI#participantView")
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

