# Dialogue Chat Bot: StackOverflow Assistant
## ONGOING Natural Language Processing Project: 
### I will be updating this project weekly or biweekly as I learn something new from the course.

I am tasked to write a bot, which will not only **answer programming-related questions**, but also will be able to **maintain a dialogue**. I am also tasked to detect the intent of the user from the question. So the first thing I need to do is to **distinguish programming-related questions from general ones**. 

Then I should find a relevant answer (a thread from StackOverflow) on a question using vector representations to calculate similarity between the question and existing threads. We already were supplied a `question_to_vec` function from the assignment 3, which can create such a representation based on word vectors. 

At the end, I should combine everything that I have done and enable the bot to maintain a dialogue. I am supposed to teach the bot to sequentially determine the intent and, depending on the intent, select the best answer. As soon as this is done, we will have the opportunity to chat with the bot and check how well it answers questions.

In addition, the chat bot should be able to handle general questions such as: "Hey", "How are you doing?", "What's your hobby?", "How to write a loop in python?", "How to delete rows in pandas?", "python3 re", "What is the difference between c and c++", "Multithreading in Java", "Catch exceptions C++", "What is AI?", etc.
