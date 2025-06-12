# 🧠 Context-Aware Gemini Chatbot (Console-Based)

This is a simple interactive chatbot that uses the **Google Gemini API** (Free or Pro) to engage in multi-turn conversations **with context awareness**. It runs in the console and allows you to adjust key model parameters for customized responses.

---

## 📌 What the Script Does

- Initializes a Gemini chat session using the `gemini-1.5-flash` model.
- Prompts the user for input in multiple turns.
- Sends each user message to the Gemini API while preserving the full conversation context.
- Lets the user **customize model behavior** by setting:
  - `temperature`
  - `top_p`
  - `max_output_tokens`
  - `frequency_penalty`
  - `presence_penalty`
- Validates all input parameters to ensure they’re in acceptable ranges.
- Provides natural back-and-forth chat experience in the console.

---

## ▶️ How to Run the Script

### ✅ 1. Setup Your Gemini API Access

Before running the script, you need a **Google API key** for the Gemini API:

1. Visit [https://makersuite.google.com/app/apikey](https://makersuite.google.com/app/apikey)
2. Generate your API key.

---

### ✅ 2. Create a `.env` File

Create a `.env` file in the **same directory** as your script with the following contents:

GEMINI_API_KEY = your_api_key_here

---

### ✅ 3. Install Python & Dependencies

Ensure you have **Python 3.7+** installed. Then, install the required library:

```bash
pip install google-generativeai python-dotenv
