# Insightify – Local AI-Powered Customer Service Chatbot

**Insightify** is a lightweight, privacy-focused AI chatbot designed to automate customer service and generate structured insights from conversations. It uses a local Large Language Model (LLM) to generate responses, logs interactions in CSV files, and is fully integrated with a React frontend for real-time user interaction.

**Demo Video**: [Watch on YouTube](https://youtu.be/y-5gViMsY8s)

---

## Features

- Local chatbot powered by a Hugging Face-hosted LLM
- React-based frontend with a clean, responsive UI
- Insight logging: captures customer name, issue, and device
- CSV-based storage (no database required)
- API endpoint (`/bot`) for message exchange
- Optional integration with Ngrok for public testing

---

## How It Works

1. The user enters a message in the frontend chat interface.
2. The message is sent to the Flask backend via the `/bot` API endpoint.
3. The backend queries a local LLM and optionally retrieves context using FAISS.
4. The generated response is returned to the frontend and displayed in the chat.
5. Customer info and interaction logs are stored in a CSV file for seller insights.

---

## Tech Stack

- Python 3
- Flask
- Hugging Face Transformers
- FAISS for vector-based context retrieval
- CSV logging (insight capture)
