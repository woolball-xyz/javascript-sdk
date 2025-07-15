# WoolballAiNetworkApi.TextGenerationApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**textGeneration**](TextGenerationApi.md#textGeneration) | **POST** /api/v1/text-generation | Text Generation - Multi-Provider

<a name="textGeneration"></a>
# **textGeneration**
> TextGenerationResponse textGeneration(provider, model, input, topK, topP, temperature, repetitionPenalty, dtype, maxLength, maxNewTokens, minLength, minNewTokens, doSample, numBeams, noRepeatNgramSize, contextWindowSize, slidingWindowSize, attentionSinkSize, frequencyPenalty, presencePenalty, bosTokenId, maxTokens, randomSeed)

Text Generation - Multi-Provider

Generate text using multiple AI providers (Transformers.js, WebLLM, MediaPipe). Use the &#x27;provider&#x27; field to specify which AI provider to use for text generation.

### Example
```javascript
import {WoolballAiNetworkApi} from 'woolball_ai_network_api';

let apiInstance = new WoolballAiNetworkApi.TextGenerationApi();
let provider = "provider_example"; // String | 
let model = "model_example"; // String | 
let input = "input_example"; // String | 
let topK = 56; // Number | 
let topP = 1.2; // Number | 
let temperature = 1.2; // Number | 
let repetitionPenalty = 1.2; // Number | 
let dtype = "dtype_example"; // String | 
let maxLength = 56; // Number | 
let maxNewTokens = 56; // Number | 
let minLength = 56; // Number | 
let minNewTokens = 56; // Number | 
let doSample = true; // Boolean | 
let numBeams = 56; // Number | 
let noRepeatNgramSize = 56; // Number | 
let contextWindowSize = 56; // Number | 
let slidingWindowSize = 56; // Number | 
let attentionSinkSize = 56; // Number | 
let frequencyPenalty = 1.2; // Number | 
let presencePenalty = 1.2; // Number | 
let bosTokenId = 56; // Number | 
let maxTokens = 56; // Number | 
let randomSeed = 56; // Number | 

apiInstance.textGeneration(provider, model, input, topK, topP, temperature, repetitionPenalty, dtype, maxLength, maxNewTokens, minLength, minNewTokens, doSample, numBeams, noRepeatNgramSize, contextWindowSize, slidingWindowSize, attentionSinkSize, frequencyPenalty, presencePenalty, bosTokenId, maxTokens, randomSeed, (error, data, response) => {
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
 **provider** | **String**|  | 
 **model** | **String**|  | 
 **input** | **String**|  | 
 **topK** | **Number**|  | 
 **topP** | **Number**|  | 
 **temperature** | **Number**|  | 
 **repetitionPenalty** | **Number**|  | 
 **dtype** | **String**|  | 
 **maxLength** | **Number**|  | 
 **maxNewTokens** | **Number**|  | 
 **minLength** | **Number**|  | 
 **minNewTokens** | **Number**|  | 
 **doSample** | **Boolean**|  | 
 **numBeams** | **Number**|  | 
 **noRepeatNgramSize** | **Number**|  | 
 **contextWindowSize** | **Number**|  | 
 **slidingWindowSize** | **Number**|  | 
 **attentionSinkSize** | **Number**|  | 
 **frequencyPenalty** | **Number**|  | 
 **presencePenalty** | **Number**|  | 
 **bosTokenId** | **Number**|  | 
 **maxTokens** | **Number**|  | 
 **randomSeed** | **Number**|  | 

### Return type

[**TextGenerationResponse**](TextGenerationResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

