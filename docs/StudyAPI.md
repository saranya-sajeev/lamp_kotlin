# StudyAPI

All URIs are relative to *https://api.lamp.digital*

Method | HTTP request | Description
------------- | ------------- | -------------
[**studyAll**](StudyAPI.md#studyAll) | **GET** /study | Get the set of all studies.
[**studyAllByResearcher**](StudyAPI.md#studyAllByResearcher) | **GET** /researcher/{researcher_id}/study | Get the set of studies for a single researcher.
[**studyCreate**](StudyAPI.md#studyCreate) | **POST** /researcher/{researcher_id}/study | Create a new Study for the given Researcher.
[**studyDelete**](StudyAPI.md#studyDelete) | **DELETE** /study/{study_id} | Delete a study.
[**studyUpdate**](StudyAPI.md#studyUpdate) | **PUT** /study/{study_id} | Update the study.
[**studyView**](StudyAPI.md#studyView) | **GET** /study/{study_id} | Get a single study, by identifier.


<a name="studyAll"></a>
# **studyAll**
> kotlin.Array&lt;kotlin.Any&gt; studyAll(transform)

Get the set of all studies.

Get the set of all studies.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = StudyAPI()
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.studyAll(transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StudyAPI#studyAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StudyAPI#studyAll")
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

<a name="studyAllByResearcher"></a>
# **studyAllByResearcher**
> kotlin.Array&lt;kotlin.Any&gt; studyAllByResearcher(researcherId, transform)

Get the set of studies for a single researcher.

Get the set of studies for a single researcher.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = StudyAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.studyAllByResearcher(researcherId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StudyAPI#studyAllByResearcher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StudyAPI#studyAllByResearcher")
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

<a name="studyCreate"></a>
# **studyCreate**
> kotlin.String studyCreate(researcherId, study)

Create a new Study for the given Researcher.

Create a new Study for the given Researcher.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = StudyAPI()
val researcherId : kotlin.String = researcherId_example // kotlin.String | 
val study : Study =  // Study | 
try {
    val result : kotlin.String = apiInstance.studyCreate(researcherId, study)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StudyAPI#studyCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StudyAPI#studyCreate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **researcherId** | **kotlin.String**|  |
 **study** | [**Study**](Study.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="studyDelete"></a>
# **studyDelete**
> kotlin.String studyDelete(studyId)

Delete a study.

Delete a study.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = StudyAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.studyDelete(studyId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StudyAPI#studyDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StudyAPI#studyDelete")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **studyId** | **kotlin.String**|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="studyUpdate"></a>
# **studyUpdate**
> kotlin.String studyUpdate(studyId, study)

Update the study.

Update the study.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = StudyAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val study : Study =  // Study | 
try {
    val result : kotlin.String = apiInstance.studyUpdate(studyId, study)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StudyAPI#studyUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StudyAPI#studyUpdate")
    e.printStackTrace()
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **studyId** | **kotlin.String**|  |
 **study** | [**Study**](Study.md)|  |

### Return type

**kotlin.String**

### Authorization


Configure Authorization:
    ApiClient.apiKey["Authorization"] = ""
    ApiClient.apiKeyPrefix["Authorization"] = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="studyView"></a>
# **studyView**
> kotlin.Array&lt;kotlin.Any&gt; studyView(studyId, transform)

Get a single study, by identifier.

Get a single study, by identifier.

### Example
```kotlin
// Import classes:
//import digital.lamp.lamp-core.infrastructure.*
//import digital.lamp.lamp-core.models.*

val apiInstance = StudyAPI()
val studyId : kotlin.String = studyId_example // kotlin.String | 
val transform : kotlin.String = transform_example // kotlin.String | 
try {
    val result : kotlin.Array<kotlin.Any> = apiInstance.studyView(studyId, transform)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StudyAPI#studyView")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StudyAPI#studyView")
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

