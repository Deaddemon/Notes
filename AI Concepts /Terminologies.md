# Table of Contents

### Resource 
- https://youtu.be/OYvlznJ4IZQ?si=s9Z68kt_LDoythS0

## Large Language Model

- A neural network that is trained to predict the next term of a input sequence
- example: Input - "All that glitters" Next term - "is not gold"

## Tokenization
(Input processing)
- Related to input of LLM, breaking the input into descrete tokens. What is the smallest term through which meaning can be driven

## Vectors 
(Input processing)
- What meaning to be drived is handled by vectors
- vectorization: similar meaning words are grouped together in a n-dimensional space and then this are turned into a coordinate
- mapping of a word in a n-dimensional space such that similar meaning words are all  clusterted together is vector
- 👉 Example:
- “happy” and “joyful” → close  
- “happy” and “sad” → far  

## Attention Mechanism
(Input processing)
- Nearby words paying addding context to the word, similar to how human derive meaning
- ex: "Tasty Apple", "Apples Revenue", "An Apple of my eye"
-  Ambigious tokens which are difficult to understand, we have mechanism to add context by looking at nearby words

## Self Supervised Learning
- Looking at text and creating multiple chalanges for yourself without human intervention, it helps to understand underlying meaning
- In self-supervised learning (especially for images), you don’t manually cut or label patches. Instead, a data preprocessing pipeline generates them on the fly during training. ex: A python code being used to generte these patches

Intent
- A student learning by filling blanks, solving puzzles, or predicting next steps
- No teacher needed—just smart exercises

## Transformer  
- A specfic Algorithm through which you predict the next token in a given input sequence.
- Input tokens -> attention block -> FFNN -> output vector -> repeat until confident

## Fine Tuning 
- If a model is trained in medical operations, it will look for next term in medical terms
- base model is trained first (transformer) -> series of ques & ans
- Process where a base model is trained to answer in a specific way is called fine tuning
- same base model can be passed through different ques & ans to come up with mutliple fine tuned models. Ex: base model llama can be fined tuned by a company to ans custom specifc queries

## Few Shot prompting 
- Few-shot prompting is a technique where you give a model a small number of examples (shots) in the prompt so it can learn the pattern and produce better outputs. Example in prompt
- English: Hello → French: Bonjour  
English: Thank you → French: Merci  
English: Good night → French:
Now the model completes it correctly.
- Use it when:
Instructions alone aren’t enough
You want a specific format
You need consistent style or reasoning
Task is slightly complex

## RAG ( Retrieval augmented generation)

- customer -> server -> company specific doc (Policy doc, T&C), Input of user, Examples -> LLM -> Response
- Retrieve the context, augment to query (enhacing input by attaching context, the docs ), generate response.
- The company doc can be stored in various location like memory(cache), GraphDB, vectorDB. usually stored in vectorDB, it is faster to fetch

## VectorDB
- store document in vector form and retrieve them when needed
- ex: "I am upset with your tool. I want refund". The word "Upset" might not be present in company documents but words like "Low rating", "user drop off" will be the closest coordinates to this.

## Model context protocol (MCP)
- communicating context to model
- ex: user -> MCP client -> LLM
  MCP cient -> MCP server (Indigo), MCP server (Air India)

## Context engineering
- few shot prompting, RAG (vector DB), MCP (external servers and perform actions)

## Agent
- long running process who can connect with LLM and external systems,  Perform tasks autonomously

## Reinforcement learning
- RLFH : reinforcement learning from human feeback, twpo responses are generated , choosen response get +1, other -1, in the n-dimensionl some vectors will be neutral, some +1, -1.

## Chain of thoughts
- train to reason step by step. ex: model giving final ans of a caluclualtion and with chain of thoughts , it gives proper step by step calculation

## Reasoning model
- not necessarily use chain of thoughts, it can use other algorithms tree of thought, graph of thought
- given a problem, a model that can reason out how to solve a problem step by step
- also known as LRMs, example: deepseek, open AI


## Multi-model models
- operate on any kind of inputs, ex: text, image, videos

## Small language models
- fewers parameters or weights (3 - 300 million)
- neural networks have fewer connections
- trained on lesser data, company specfic or task specific

## Distillation
- process of building SML 

## Quantization
- Reduces model size by lowering precision:
  - Example: 32-bit → 8-bit

👉 Benefits:
- Faster inference  
- Lower memory usage  

