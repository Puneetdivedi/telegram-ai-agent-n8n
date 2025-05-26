# 🔐 Credential Setup Guide

## 1. Telegram
- Talk to [BotFather](https://t.me/botfather)
- Create a new bot and copy the token
- In n8n, go to **Credentials > Telegram API** and paste the token

## 2. OpenAI
- Go to https://platform.openai.com/account/api-keys
- Generate a new API key
- In n8n, add a new credential of type **OpenAI**

## 3. SerpAPI (Optional)
- Go to https://serpapi.com/
- Sign up and get your API key
- Add it in n8n credentials as **SerpAPI**

## Testing
- Import the workflow (`telegram-ai-agent.json`)
- Set your credentials in each node
- Activate the workflow and start messaging your bot!
