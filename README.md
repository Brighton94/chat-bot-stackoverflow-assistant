# Dialogue Chatbot: StackOverflow Assistant
## Natural Language Processing Project. 

The main focus of projects to build and built here are task-oriented dialog systems like Apple Siri or Amazon Alexa. I have currently wrote a chatbot which is not only able to answer **_programming-related questions_**, but also **_maintain a dialogue_**. In a nutshell, I first had to detect the intent of the user from the question; so I had to **_distinguish programming-related questions from general ones_**. 

Secondly, I had to find a relevant answer (a thread from StackOverflow) on a question using vector representations to calculate similarity between the question and existing threads. So the idea was to convert a question into a vector and calculate the cosine similarity, for instance, with thread vectors. 

Lastly, I combined everything that I have done and enabled the bot to maintain a dialogue. I trained/taught the bot to sequentially determine the intent and, depending on the intent, select the best answer. As soon as this was done, I had the have the opportunity to chat with the bot and check how well it answers both programming-related and general questions such as: "Hey", "How are you doing?", "What's your hobby?", "How to write a loop in python?", "How to delete rows in pandas?", "python3 re", "What is the difference between c and c++", "Multithreading in Java", "Catch exceptions C++", "What is AI?", etc.

## Possible next steps: Custom Chatbot

1. Build a **_Telegram chatbot_** hosted on AWS or on Flask to get a web-server that servers as a chatbot
and/or
2. **_build a custom chatbot_**. There are various recommendations to consider when building a custom chatbot:
  - Generative model: n-gram language model.
  - Generative model: LSTM-based language model.
  - Conditional language modeling: seq2seq model.
  - Selective model: embeddings-based ranking.
  - Selective model: DSSM.

Also, one thing to note about dialogue chatbots is that choosing the right dataset to train them can make a big difference.
