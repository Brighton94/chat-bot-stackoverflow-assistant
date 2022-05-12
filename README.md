# Dialogue Chatbot: StackOverflow Assistant
## Natural Language Processing Project. 

The main focus here are task-oriented dialog systems like Apple Siri or Amazon Alexa. I have currently wrote a chatbot which is not only able to answer **_programming-related questions_**, but also **_maintain a dialogue_**. In a nutshell, I first had to detect the intent of the user from the question; so I had to **_distinguish programming-related questions from general ones_**. 

Secondly, I had to find a relevant answer (a thread from StackOverflow) on a question using vector representations to calculate similarity between the question and existing threads. So the idea was to convert a question into a vector and calculate the cosine similarity, for instance, with thread vectors. 

Lastly, I combined everything that I have done and enabled the bot to maintain a dialogue. I trained/taught the bot to sequentially determine the intent and, depending on the intent, select the best answer. As soon as this was done, I had the have the opportunity to chat with the bot and check how well it answers both programming-related and general questions such as: "Hey", "How are you doing?", "What's your hobby?", "How to write a loop in python?", "How to delete rows in pandas?", "python3 re", "What is the difference between c and c++", "Multithreading in Java", "Catch exceptions C++", "What is AI?", etc.

## Possible next steps: Custom Chatbot and Telegram Chatbot

1. Build a **_Telegram chatbot_** hosted on AWS or on Flask to get a web-server that servers as a chatbot
and/or
2. **_build a custom chatbot_**. There are various recommendations to consider when building a custom chatbot:
  - Generative model: n-gram language model.
  - Generative model: LSTM-based language model.
  - Conditional language modeling: seq2seq model.
  - Selective model: embeddings-based ranking.
  - Selective model: eep Structures Semantic Model (DSSM).

Also, one thing to note about dialogue chatbots is that choosing the right dataset to train them can make a big difference.

Here are a few dialogue datasets to train the models that were recommended:

  - [Cornell Movie Dialogs](https://www.cs.cornell.edu/%7Ecristian/Cornell_Movie-Dialogs_Corpus.html) - small corpus of dialogues from English movies.

  - [OpenSubtitles](https://opus.nlpl.eu/OpenSubtitles.php) - bigger corpus of English subtitles (but also noisier).

There are a a [set of tools](https://github.com/Brighton94/chat-bot-stackoverflow-assistant/tree/main/download_read_utils) that were provided for working with these datasets. This includes shell scripts for downloading raw data, Python library for reading it into memory and a simple [example](https://github.com/Brighton94/chat-bot-stackoverflow-assistant/blob/main/example.py) to show how to use it. Note, that the [datasets](https://github.com/Brighton94/chat-bot-stackoverflow-assistant/blob/main/download_read_utils/datasets.py) library already performs data tokenization, filtering of long sentences and splitting conversations into pairs of sentences that will serve as training data for your chat-bot. However, feel free to change any of those bits as you see fit.

More conversational datasets can be found [here](https://github.com/Conchylicultor/DeepQA#presentation).
