# ActivityAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activityAll**](ActivityAPI.md#activityAll) | **GET** /activity | Get the set of all activities.
[**activityAllByParticipant**](ActivityAPI.md#activityAllByParticipant) | **GET** /participant/{participant_id}/activity | Get all activities for a participant.
[**activityAllByResearcher**](ActivityAPI.md#activityAllByResearcher) | **GET** /researcher/{researcher_id}/activity | Get all activities for a researcher.
[**activityAllByStudy**](ActivityAPI.md#activityAllByStudy) | **GET** /study/{study_id}/activity | Get all activities in a study.
[**activityCreate**](ActivityAPI.md#activityCreate) | **POST** /study/{study_id}/activity | Create a new Activity under the given Study.
[**activityDelete**](ActivityAPI.md#activityDelete) | **DELETE** /activity/{activity_id} | Delete an Activity.
[**activityUpdate**](ActivityAPI.md#activityUpdate) | **PUT** /activity/{activity_id} | Update an Activity&#39;s settings.
[**activityView**](ActivityAPI.md#activityView) | **GET** /activity/{activity_id} | Get a single activity, by identifier.


<a name="activityAll"></a>
# **activityAll**
> kotlin.Array&lt;kotlin.Any&gt; activityAll(transform)

Get the set of all activities.

Get the set of all activities.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityAPI()
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activityAll(transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPI#activityAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPI#activityAll")
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

<a name="activityAllByParticipant"></a>
# **activityAllByParticipant**
> kotlin.Array&lt;kotlin.Any&gt; activityAllByParticipant(participantId, transform)

Get all activities for a participant.

Get the set of all activities available to a participant, by  participant identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityAPI()
val participantId : kotlin.String = participantId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activityAllByParticipant(participantId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPI#activityAllByParticipant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPI#activityAllByParticipant")
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

<a name="activityAllByResearcher"></a>
# **activityAllByResearcher**
> kotlin.Array&lt;kotlin.Any&gt; activityAllByResearcher(researcherId, transform)

Get all activities for a researcher.

Get the set of all activities available to participants of any study  conducted by a researcher, by researcher identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activityAllByResearcher(researcherId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPI#activityAllByResearcher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPI#activityAllByResearcher")
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

<a name="activityAllByStudy"></a>
# **activityAllByStudy**
> kotlin.Array&lt;kotlin.Any&gt; activityAllByStudy(studyId, transform)

Get all activities in a study.

Get the set of all activities available to  participants of a single  study, by study identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activityAllByStudy(studyId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPI#activityAllByStudy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPI#activityAllByStudy")
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

<a name="activityCreate"></a>
# **activityCreate**
> kotlin.String activityCreate(studyId, activity)

Create a new Activity under the given Study.

Create a new Activity under the given Study.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val activity : Activity =  // Activity | 
try {
    val result : kotlin.String = apiInstance.activityCreate(studyId, activity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPI#activityCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPI#activityCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **studyId** | **kotlin.String**|  |
 **activity** | [**Activity**](Activity.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="activityDelete"></a>
# **activityDelete**
> kotlin.String activityDelete(activityId)

Delete an Activity.

Delete an Activity.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityAPI()
val activityId : kotlin.String = activityId_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.activityDelete(activityId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPI#activityDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPI#activityDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activityId** | **kotlin.String**|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="activityUpdate"></a>
# **activityUpdate**
> kotlin.String activityUpdate(activityId, activity)

Update an Activity&#39;s settings.

Update an Activity&#39;s settings.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityAPI()
val activityId : kotlin.String = activityId_example // kotlin.String | 
val activity : Activity =  // Activity | 
try {
    val result : kotlin.String = apiInstance.activityUpdate(activityId, activity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPI#activityUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPI#activityUpdate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activityId** | **kotlin.String**|  |
 **activity** | [**Activity**](Activity.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="activityView"></a>
# **activityView**
> kotlin.Array&lt;kotlin.Any&gt; activityView(activityId, transform)

Get a single activity, by identifier.

Get a single activity, by identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = ActivityAPI()
val activityId : kotlin.String = activityId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.activityView(activityId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPI#activityView")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPI#activityView")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activityId** | **kotlin.String**|  |
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

