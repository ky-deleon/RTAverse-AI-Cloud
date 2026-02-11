# 🚦 RTAverse AI (Cloud Version)

> **A Machine Learning-Based Road Traffic Accident Forecasting System**

RTAverse AI is an intelligent assistant designed to analyze traffic patterns and accident forecasting data. Powered by **Meta's Llama 3** and **Retrieval-Augmented Generation (RAG)**, this system allows users to "chat" with the RTAverse thesis paper and source code to gain insights into accident hotspots and forecasting algorithms.

This version is optimized to run entirely in the cloud using **Google Colab (Tesla T4 GPU)** and serves a web interface via **Ngrok**.

---

## ✨ Key Features

* **🧠 Advanced LLM:** Utilizes `Meta-Llama-3-8B-Instruct` (4-bit quantized) for high-quality, natural language responses.
* **📚 RAG Architecture:** Context-aware answers based on the loaded thesis PDF and codebase.
* **💬 Interactive Web UI:** A custom Flask-based chat interface with Dark/Light mode, built-in summarization, and source citation.
* **☁️ Cloud-Native:** Runs on Google Colab's free tier GPU; no local hardware required.
* **ww Secure Tunneling:** Instantly accessible from any device via an auto-generated Ngrok link.

## 🛠️ Tech Stack

* **Core:** Python 3.10+
* **AI/ML:** Hugging Face Transformers, LangChain, ChromaDB, BitsAndBytes
* **Web Framework:** Flask (Backend), HTML/CSS/JS (Frontend)
* **Infrastructure:** Google Colab, PyNgrok

## 🚀 How to Run

### Prerequisites
1.  **Google Account** (for Colab).
2.  **Hugging Face Account** (with a generic `READ` token).
3.  **Ngrok Account** (for the free authtoken).

### Step-by-Step Guide

1.  **Open in Colab:**
    Open the `.ipynb` file in Google Colab.
    
2.  **Set Up Secrets:**
    On the left sidebar of Colab, click the **Key icon (Secrets)** and add the following keys:
    * `HF_TOKEN`: Your Hugging Face Access Token.
    * `NGROK_TOKEN`: Your Ngrok Authtoken.
    *(Toggle "Notebook access" to ON for both).*

3.  **Run the Notebook:**
    Go to **Runtime > Run all**. The system will:
    * Install dependencies.
    * Load the Llama 3 model.
    * Index the thesis PDF and code files.
    * Start the Flask server.

4.  **Launch the App:**
    Scroll to the final cell output and click the link ending in `.ngrok-free.app` (e.g., `https://a1b2-c3d4.ngrok-free.app`).

## ⚠️ Important Notes

* **Session Timeout:** Google Colab runtimes disconnect after a period of inactivity. If the app stops working, simply restart the runtime in Colab.
* **Data Safety:** Do not upload sensitive personal data to the chat interface, as the session is temporary.
