# 🤖 Telegram AI Agent with n8n

## 📌 Description
This project creates an intelligent Telegram bot using [n8n](https://n8n.io/) and integrates it with **OpenAI**, **LangChain**, and **SerpAPI** to provide smart, context-aware responses. It supports handling both **text** and **voice** messages (filtered with a Switch node).

## 🛠️ Technologies Used
- 🔁 [n8n](https://n8n.io/) – Automation and workflow orchestration
- 🤖 OpenAI (GPT-4o-mini) – AI responses
- 🧠 LangChain – Agent + memory management
- 🔍 SerpAPI – Real-time web search capability
- 💬 Telegram Bot API – Messaging interface

## 🚀 How It Works
1. User sends a message to a Telegram bot.
2. n8n triggers on new message via the `telegramTrigger` node.
3. A `Switch` node detects if the message is voice or text.
4. If text, it's routed through the LangChain Agent which:
   - Uses OpenAI to generate replies
   - Maintains chat memory per session
   - Optionally queries SerpAPI for real-time info
5. Response is sent back to Telegram.

## 📂 File Structure
