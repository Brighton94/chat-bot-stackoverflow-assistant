# Dialogue Chatbot: StackOverflow Assistant
## Natural Language Processing Project. 

I was tasked to write a bot, which will not only **answer programming-related questions**, but also will be able to **maintain a dialogue**. I was also tasked to detect the intent of the user from the question. So the first thing I had to do was to **distinguish programming-related questions from general ones**. 

Afterwards, I had to find a relevant answer (a thread from StackOverflow) on a question using vector representations to calculate similarity between the question and existing threads. From the previous assingment, the `question_to_vec` function was able to create such a representation based on word vectors.  

At the end, I combined everything that I have done and enabled the bot to maintain a dialogue. I trained/taught the bot to sequentially determine the intent and, depending on the intent, select the best answer. As soon as this was done, I had the have the opportunity to chat with the bot and check how well it answers both programming-related and general questions such as: "Hey", "How are you doing?", "What's your hobby?", "How to write a loop in python?", "How to delete rows in pandas?", "python3 re", "What is the difference between c and c++", "Multithreading in Java", "Catch exceptions C++", "What is AI?", etc.

As a next step of this project, I could build a Telegram chatbot hosted on AWS or on Flask to get a web-server that servers as a chatbot.
