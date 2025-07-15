# WoolballAiNetworkApi.TextGenerationRequestContract

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**provider** | **String** | The AI provider to use | 
**model** | **String** | The AI model to use for processing | 
**input** | **String** | Input text or messages for generation | 
**topK** | **Number** | The number of highest probability vocabulary tokens to keep for top-k-filtering | [optional] 
**topP** | **Number** | If set to float &lt; 1, only the smallest set of most probable tokens with probabilities that add up to top_p or higher are kept for generation | [optional] 
**temperature** | **Number** | The value used to modulate the next token probabilities | [optional] 
**repetitionPenalty** | **Number** | Parameter for repetition penalty. 1.0 means no penalty | [optional] 
**dtype** | **String** | Quantization level (e.g., &#x27;fp16&#x27;, &#x27;q4&#x27;, &#x27;q8&#x27;) - Transformers only | [optional] 
**maxLength** | **Number** | Maximum length the generated tokens can have - Transformers only | [optional] 
**maxNewTokens** | **Number** | Maximum number of tokens to generate - Transformers only | [optional] 
**minLength** | **Number** | Minimum length of the sequence to be generated - Transformers only | [optional] 
**minNewTokens** | **Number** | Minimum numbers of tokens to generate - Transformers only | [optional] 
**doSample** | **Boolean** | Whether to use sampling - Transformers only | [optional] 
**numBeams** | **Number** | Number of beams for beam search - Transformers only | [optional] 
**noRepeatNgramSize** | **Number** | If &gt; 0, all ngrams of that size can only occur once - Transformers only | [optional] 
**contextWindowSize** | **Number** | Size of the context window for the model - WebLLM only | [optional] 
**slidingWindowSize** | **Number** | Size of the sliding window for attention - WebLLM only | [optional] 
**attentionSinkSize** | **Number** | Size of the attention sink - WebLLM only | [optional] 
**frequencyPenalty** | **Number** | Penalty for token frequency - WebLLM only | [optional] 
**presencePenalty** | **Number** | Penalty for token presence - WebLLM only | [optional] 
**bosTokenId** | **Number** | Beginning of sequence token ID - WebLLM only | [optional] 
**maxTokens** | **Number** | Maximum number of tokens to generate - MediaPipe only | [optional] 
**randomSeed** | **Number** | Random seed for reproducible results - MediaPipe only | [optional] 

<a name="ProviderEnum"></a>
## Enum: ProviderEnum

* `transformers` (value: `"transformers"`)
* `webllm` (value: `"webllm"`)
* `mediapipe` (value: `"mediapipe"`)

