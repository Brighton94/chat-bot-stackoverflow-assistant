# Dialogue Chat Bot: StackOverflow Assistant
[ONGOING Natural Language Processing (NLP) Project] I will be updating this project weekly or biweekly as I learn something new from the course.

I am tasked to write a bot, which will not only answer programming-related questions, but also will be able to maintain a dialogue. I am also tasked to detect the intent of the user from the question (we could have had a 'Question answering mode' check-box in the bot, but it wouldn't fun at all, would it?). So the first thing I need to do is to distinguish programming-related questions from general ones. 

Then I should find a relevant answer (a thread from StackOverflow) on a question using vector representations to calculate similarity between the question and existing threads. We already were supplied a `question_to_vec` function from the assignment 3, which can create such a representation based on word vectors.
