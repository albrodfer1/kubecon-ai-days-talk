# Ollama

## Slide 1

### Ollama

- Ollama is a framework for running LLM models locally

### Models

- we are going to discuss models to help moderating prompts and answers to and from LLMs

## Slide 2

### shieldgemma

- set of instructions tuned models for evaluating the safety of text prompt input and output
- it contains a set of defined policies
- built upon gemma 2 (Google's model)
- categories:
  - sexually explicit
  - dangerous content
  - hate
  - harassment

## Slide 3

### granite3-guardian

- IBM
- detects risk in prompts and/or responses
- helps with risk detection along many key dimensions catalogued in [IBM AI Risk Atlas](https://www.ibm.com/docs/en/watsonx/saas?topic=ai-risk-atlas)
- 2B or 8B model
- uses:
  - risk detection in prompt or model response
    - harm
    - social bias
    - jailbreaking
    - violenece
    - profanity
    - sexual content
    - unethical behavior
  - RAG to assess (TODO: add it to notebook)
    - context relevance
    - groundedness
    - answer relevance
    
## Slide 4

### llama-guard3

- content safety classification
- prompt responses
- 1B or 8B
- safety labels
  - violent crimes
  - non violent crimes
  - sex related crimes
  - child secual exploitation
  - defamation
  - specialized advice
  - privacy
  - intellectual property
  - indiscrimanate weapons
  . hate
  - suicide & self-harm
  - sexual content
  - elections
- supported languages
  - English
  - French
  - German
  - Hindi
  - Italian
  - Portuguese
  - Spanish
  - Thai