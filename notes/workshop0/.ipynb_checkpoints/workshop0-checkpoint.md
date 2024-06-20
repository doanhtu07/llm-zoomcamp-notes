# Workshop 0

Link: https://www.youtube.com/watch?v=q-p36Ak6YI8

## LLM

Normal LLM:

- Text -> LLM -> Next token/text

  - Example: "How are" -> "you"

- Can view LLM as blackbox that given some prompts (input), it can generate a response (output)

## RAG

- RAG: Retrieval-Augmented Generation

  - A prompt like "look up how to fry an onion"
  - GPT will go up the Internet and actually use search engines
  - Then, use the retrieved information to help with generation

- When user has a question:

  - we actually look up the question in a database (GPT look up the index of the whole Internet with Bing for instance)
  - in our case, we can put the questions and answers in our database and use that to look up
  - database will give back some results
  - we then form a prompt with the user question and the context (consisting of results from database) and ask LLM to generate an answer to user question

![ Demo Image ](./map.png)

<img src="./map.png" alt="drawing" width="600px" style="display: block; margin-left: auto; margin-right: auto; margin-top: 20px; margin-bottom: 20px;" />

## Installation

- `docker run hello-world`
- `pip install pipenv`
