<div>
    <img src="https://github.com/DmitryTatarintsev/Telegram-bot/header.jpg" alt="альтернативный текст" title="заголовок изображения" width="100%" style="float: left; margin-right: 10px">
</div>

# Telegram bot for Coffee Recommendations
## Description
This project is an asynchronous Telegram bot designed to provide coffee shop recommendations based on geographic location. The bot analyzes user requests and, using the OpenAI API, suggests the best coffee shops (according to GPT) in the specified city. The project was implemented in Python, combining the capabilities of the aiogram and LangChain frameworks.

## Peculiarities
- **Asynchrony:** The bot works asynchronously, processing both incoming messages from Telegram and requests to the OpenAI API, which ensures fast and efficient interaction with the user.
- **Coffee Shop Recommendations:** The bot analyzes the specified city and offers a list of the best coffee shops, including information about the name, link to Google Maps, average bill and features of each coffee shop.
- **Memory for Each User:** To ensure contextualized communication and user convenience, a memory system has been introduced that allows you to save the history of each user’s interactions with the bot.
- **Ease of Interaction:** A simple and clear interface that makes using the bot convenient and intuitive.
## How to use
1. Send the bot a message with the name of the city where you want to find a coffee shop.
2. The bot will process your request and offer a list of recommended coffee shops.
3. You can ask clarifying questions and receive additional information about each coffee shop.

## Local Run
To run this bot locally, you need to set environment variables for OpenAI and Telegram API tokens.

### Setting Environment Variables
###Windows
Open a command prompt and use the following commands to set environment variables:
```
set OPENAI_API_KEY=your-openai-api-key
set TELEGRAM_API_TOKEN=your-telegram-token
```
###Linux
Open a terminal and use the following commands to set environment variables:

```
export OPENAI_API_KEY=your-openai-api-key
export TELEGRAM_API_TOKEN=your-telegram-token
```

### Launch the Bot
Make sure that your configuration file (config.yaml) contains the names of the environment variables, or if they have already been set, then simply enter their names:
```
openai_token_name: 'OPENAI_API_KEY'
telegram_api_token_name: 'TELEGRAM_API_TOKEN'
```
### Run the bot using Python via your command line or terminal:

```
python telegram.py
```

## Technologies
- **Python**
- **aiogram** for interaction with the Telegram API
- **LangChain** for OpenAI integration and natural language query processing
License
[Specify license type]
