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

## Finae Tuning 

