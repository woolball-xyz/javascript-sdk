# WoolballAiNetworkApi.TranslationApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**translation**](TranslationApi.md#translation) | **POST** /api/v1/translation | Translation

<a name="translation"></a>
# **translation**
> TranslationResponse translation(model, dtype, input, srcLang, tgtLang)

Translation

Translate text between 200+ languages using NLLB models. Uses FLORES200 format for language codes.

### Example
```javascript
import {WoolballAiNetworkApi} from 'woolball_ai_network_api';

let apiInstance = new WoolballAiNetworkApi.TranslationApi();
let model = "model_example"; // String | 
let dtype = "dtype_example"; // String | 
let input = "input_example"; // String | 
let srcLang = "srcLang_example"; // String | 
let tgtLang = "tgtLang_example"; // String | 

apiInstance.translation(model, dtype, input, srcLang, tgtLang, (error, data, response) => {
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
 **srcLang** | **String**|  | 
 **tgtLang** | **String**|  | 

### Return type

[**TranslationResponse**](TranslationResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

