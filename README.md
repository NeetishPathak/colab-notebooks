## LLM Biz Class Notes

Grok 4 - best for reasoning 

Models for the skills and not the knowledge 
	Skill ----- Writing code, Summarization, 
	NOT Knowledge ----- X


Pre 2013 - One hot Encding 
	- No rlnshp of simialrity captured

Word2Vec : Word embeddings (musical notes)
	Symantically similarity
Representing a word by means of its neighbors 

CBOW 
Skip-gram 

https://projector.tensorflow.org/

Reduce the dimensions PCA

RNN, LSTM (Long Short term memory)
John went to the store. He ---> (should refer to John but in LSTM , this is gone)

Attention is all you need
Transformer ( He and John would higher weighting ) - generalization

Encoding Decoding 
Attention Maps
Transformer


Token Embeddings
Tokens ---> Number 

Auto regressive prediction process 
	max prediction tokens
	 End of line ytoken s

	Word to Token (numer) to embedding 

NBER call center study
Leveling up 
Complain resolution

Jama Network Open 
Findings 76%  with chabot ai and 74% without 

Golden Gate Claude - https://www.anthropic.com/news/golden-gate-claude

Prompt Engineering 
- Think like a detective
- Give example! Provide context and direction 
- Refine and adjust: Experiment and improve
- List Example: Include specific examples of prompts for different tasks

R - Role define a specific role. You are a cybersecurity expert. IQ of 125
I - Instruction - Give direct command. Analyze the security vulnerabilities in this network
S - Steps - Break into logical parts. Identify outdated software. List potential security threats. Recommend fixes
E - Examples - Provide an expected response format. A good report should include bullet points and a risk severity rating.
N - Narrowing - Restrict scope, length or complexity. Example: Focus only on firewall vulnerabilities.Limit response to 200 words.


Give the permission to be wrong 


Being more firmer and stricter

Prompt injection is the process of hijacking a language models
It allows the hacker to get the model to say anything that they want.

Delimiter 
Anthropic works better with tags
Chat gpt works better with back ticks

```
<Role> You are a tech analyst with an IQ of 123</Role>
<Instruction> You are supposed to analyse metrics for latency and give me the avg, p50, p99, p9999 </<Instruction>
<Input> [2.8,4,3,2,4,2,1,8.9,7.6]</Input>
<Steps>
<Step1>Mean of latencies</Step1>
<Step1>p50 of latencies</Step1>
<Step1>p99 of latnecies</Step1>
<Steps>
<Scope>only Give latencies in propely formatted manner with emoticons</Scope>
```

### Zero Shot prompting 
No examples but give more examples, few short prompting 

input_text = """ 
Classify the text as neutral, negative, or positive. your response should be one word. 
Text: I think the vacation is okay
Sentiment: 
"""

Textbooks are all you need Paper: https://arxiv.org/pdf/2306.11644

Chatmode in chatgpt api platform


Chain of thought : Break down complex tasks 
Model text 
Chain of Through
Q:
A:
Q:

A

gpt-41 is not 
o4-mini is the reasoning mode


RAG (Retrieval Augmented generations)
Scaling RAG is extremely difficulyt 
- Invest In building knowledge source 

gpt-2 encoder
https://github.com/Accentax/gpt-2/blob/master/src/encoder.py
