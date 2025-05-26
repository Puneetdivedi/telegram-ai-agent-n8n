# 📊 Architecture Overview

1. Telegram message triggers the n8n webhook.
2. Switch node checks if the message is text or voice.
3. If text, it's routed through a LangChain AI Agent node.
4. Agent uses OpenAI (GPT-4o-mini) for response generation.
5. A memory node stores short-term context per session.
6. If needed, SerpAPI is used to get real-time data.
7. The response is sent back to the user via Telegram.
