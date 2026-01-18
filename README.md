# n8n-roas-automation
This project is an **end-to-end ROAS automation system** built using **n8n**, designed for **media buying teams** to automatically:  - Fetch ROAS data from Google Sheets - Clean and normalize financial metrics - Match brands with account handlers - Send personalized performance reports via WhatsApp
---

## 🚀 Features

- ✅ Multi-sheet Google Sheets integration
- ✅ Dynamic brand & handler detection (Row-based configuration)
- ✅ Robust data cleaning (currency, errors, nulls)
- ✅ Daily ROAS, spending & sales reporting
- ✅ WhatsApp message automation
- ✅ Batch processing with random delays (anti-spam)
- ✅ Modular Python & JavaScript logic inside n8n

---

## 🧠 How It Works

1. **Google Sheets Nodes**
   - Pull ROAS data for multiple buyers
   - Fetch handler contact lists

2. **Python Code Nodes**
   - Parse brand + handler definitions
   - Clean numeric values (Rs, %, errors)
   - Filter data by processing date
   - Generate structured performance records

3. **JavaScript Code Nodes**
   - Match brands with WhatsApp contacts
   - Format human-readable messages
   - Prepare WhatsApp payloads

4. **HTTP Request Node**
   - Sends performance reports via WhatsApp API

---

## 🛠 Tech Stack

- **n8n**
- **Python (Native n8n Code Nodes)**
- **JavaScript**
- **Google Sheets API**
- **WhatsApp Cloud / WA Web API**

---

## 🔐 Environment Variables

Create a `.env` file:

```env
WHATSAPP_INSTANCE_ID=YOUR_INSTANCE_ID
WHATSAPP_ACCESS_TOKEN=YOUR_ACCESS_TOKEN
GOOGLE_SHEET_ID=YOUR_GOOGLE_SHEET_ID
