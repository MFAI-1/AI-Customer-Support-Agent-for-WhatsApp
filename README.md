#  WhatsApp AI Customer Support Agent
Transform your customer service with an AI-powered WhatsApp agent that works 24/7, responds instantly, and handles unlimited conversations simultaneously. This automation reduces response times from hours to seconds, improves customer satisfaction, and frees up your human agents for complex issues - all while saving your business thousands in operational costs.
<img width="1682" height="856" alt="Advance Whatsapp Agent" src="https://github.com/user-attachments/assets/46d6bb93-ff05-4386-8ec4-66ce2fdbe014" />

[![n8n](https://img.shields.io/badge/n8n-0.234.0-ff6b6b?style=flat-square&logo=n8n)](https://n8n.io)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-412991?style=flat-square&logo=openai)](https://openai.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![Automation](https://img.shields.io/badge/Automation-AI%20Agent-blue?style=flat-square)](https://github.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Business%20API-25D366?style=flat-square&logo=whatsapp)](https://developers.facebook.com/docs/whatsapp)

> **AI-powered WhatsApp customer support agent that automatically responds to customer inquiries using OpenAI's GPT-4**

---

## ✨ Features

- 🤖 **AI-powered responses** using OpenAI GPT-4
- 📱 **WhatsApp Business API integration** for seamless communication
- 🔄 **Real-time message processing** with automatic responses
- 🎯 **Intelligent conversation handling** with context awareness
- ⚡ **Scalable architecture** for high-volume customer interactions
- 🛡️ **Error handling** and fallback responses
- 📊 **Conversation tracking** for customer insights
- 🔧 **Easy customization** for different business needs

---

## 📋 Workflow Overview

This n8n workflow connects WhatsApp Business API with OpenAI's GPT-4 to create an intelligent customer support agent. When a customer sends a message to your WhatsApp Business number, the workflow:

1. **Receives** the incoming message via webhook
2. **Processes** the message content
3. **Sends** the query to OpenAI's GPT-4 with context
4. **Generates** a personalized, helpful response
5. **Sends** the response back to the customer via WhatsApp

The system maintains conversation context to provide coherent, contextual responses throughout the conversation.

---

## 🔧 How It Works

### Workflow Flow

1. **WhatsApp Webhook Trigger** - Listens for incoming messages
2. **Message Processing** - Extracts sender info and message content
3. **Context Retrieval** - Fetches conversation history (if applicable)
4. **AI Processing** - Sends to OpenAI with system prompt
5. **Response Generation** - Creates natural, helpful response
6. **WhatsApp Reply** - Sends response back to customer

---

## 📋 Requirements

- **n8n Version**: 0.234.0 or higher
- **Required APIs**:
  - WhatsApp Business API
  - OpenAI API
- **Required Accounts**:
  - Meta/Facebook Developer Account
  - WhatsApp Business Account
  - OpenAI Account
- **Required Credentials**:
  - WhatsApp Access Token
  - WhatsApp Phone Number ID
  - OpenAI API Key

---

## 🔐 Environment Variables

```bash
WHATSAPP_ACCESS_TOKEN=your_whatsapp_access_token
WHATSAPP_PHONE_NUMBER_ID=your_phone_number_id
OPENAI_API_KEY=your_openai_api_key
OPENAI_MODEL=gpt-4
SYSTEM_PROMPT=You are a helpful customer support agent...
