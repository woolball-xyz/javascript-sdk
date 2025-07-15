# WoolballAiNetworkApi.SpeechRecognitionApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**speechToText**](SpeechRecognitionApi.md#speechToText) | **POST** /api/v1/speech-recognition | Speech Recognition (Speech-to-Text)

<a name="speechToText"></a>
# **speechToText**
> [STTChunk] speechToText(model, dtype, input, returnTimestamps, stream, chunkLengthS, strideLengthS, forceFullSequences, language, task, numFrames)

Speech Recognition (Speech-to-Text)

Convert audio files to text using Whisper models. Supports MP3, WAV, M4A and other audio formats.

### Example
```javascript
import {WoolballAiNetworkApi} from 'woolball_ai_network_api';

let apiInstance = new WoolballAiNetworkApi.SpeechRecognitionApi();
let model = "model_example"; // String | 
let dtype = "dtype_example"; // String | 
let input = null; // Object | 
let returnTimestamps = "returnTimestamps_example"; // String | 
let stream = true; // Boolean | 
let chunkLengthS = 56; // Number | 
let strideLengthS = 56; // Number | 
let forceFullSequences = true; // Boolean | 
let language = "language_example"; // String | 
let task = "task_example"; // String | 
let numFrames = 56; // Number | 

apiInstance.speechToText(model, dtype, input, returnTimestamps, stream, chunkLengthS, strideLengthS, forceFullSequences, language, task, numFrames, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model** | **String**|  | 
 **dtype** | **String**|  | 
 **input** | [**Object**](.md)|  | 
 **returnTimestamps** | **String**|  | 
 **stream** | **Boolean**|  | 
 **chunkLengthS** | **Number**|  | 
 **strideLengthS** | **Number**|  | 
 **forceFullSequences** | **Boolean**|  | 
 **language** | **String**|  | 
 **task** | **String**|  | 
 **numFrames** | **Number**|  | 

### Return type

[**[STTChunk]**](STTChunk.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

