# Running Shoes Recommender Chat Bot

This project aims to help users find running shoes which are similar to their favourite pair of running shoes.

## Goal

Based on a given pair of running shoes chosen by the user, recommend a set of running shoes that have similar features.

## Dataset

Data of running shoes was scraped from [RunRepeat](https://runrepeat.com/).

## Approach

The recommender is built on content-based filtering. Separate scores are generated for similarities in shoe feature, rating, popularity and review. Subsequently, the scores are aggregated to a final score, which would determine which shoes would be recommended to the user.

## Tools
This chatbot is built using Rasa, an open-source machine learning framework for buidling chatbots. Rasa consists of two modules, namely Rasa Natural Language Understanding(NLU) for understanding users' messages and extracting important information, and Rasa Core for predicting the next action for the chatbot. Python package [Levenshtein](https://rawgit.com/ztane/python-Levenshtein/master/docs/Levenshtein.html) was used to handle spelling errors or typo errors by finding the closest shoe name to the shoe names in the database.

## Implementation
The chatbot is deployed on Telegram [(@running_shoes_bot)](https://t.me/running_shoes_bot).

## References
- [Rasa](https://rasa.com/docs/rasa/)
- [Telegram bot](https://core.telegram.org/bots)
- [Levenshtein](https://rawgit.com/ztane/python-Levenshtein/master/docs/Levenshtein.html)