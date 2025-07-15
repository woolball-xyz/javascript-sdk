# WoolballAiNetworkApi.TextToSpeechApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**textToSpeech**](TextToSpeechApi.md#textToSpeech) | **POST** /api/v1/text-to-speech | Text-to-Speech

<a name="textToSpeech"></a>
# **textToSpeech**
> [TTSResponse] textToSpeech(model, dtype, input, voice, stream)

Text-to-Speech

Generate natural speech from text using MMS or Kokoro models. Supports multiple languages and premium voices.

### Example
```javascript
import {WoolballAiNetworkApi} from 'woolball_ai_network_api';

let apiInstance = new WoolballAiNetworkApi.TextToSpeechApi();
let model = "model_example"; // String | 
let dtype = "dtype_example"; // String | 
let input = "input_example"; // String | 
let voice = "voice_example"; // String | 
let stream = true; // Boolean | 

apiInstance.textToSpeech(model, dtype, input, voice, stream, (error, data, response) => {
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
 **input** | **String**|  | 
 **voice** | **String**|  | 
 **stream** | **Boolean**|  | 

### Return type

[**[TTSResponse]**](TTSResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

