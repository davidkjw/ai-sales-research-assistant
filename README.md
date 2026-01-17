# 🔍 AI Sales Research Assistant - Local (Ollama)

[![Ollama](https://img.shields.io/badge/LLM-Ollama-orange)](https://ollama.ai/)
[![Status](https://img.shields.io/badge/Status-Functional_PoC-brightgreen)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**A high-performance, 100% private sales intelligence suite that runs entirely on your local hardware. No API costs, no cloud data leaks, and zero subscriptions.**

---

## 🎯 The "PoC-to-Production" Bridge

Most AI sales tools require expensive OpenAI/Claude API keys and send your sensitive prospect data to the cloud. This assistant bridges that gap by using a **Client-Side Orchestration** model:

* **🛡️ Data Sovereignty**: Unlike cloud-based SaaS, your prospect lists and talk tracks never leave your local machine.
* **⚡ Zero-Latency UI**: Built as a single-file React/Tailwind app that communicates directly with the Ollama local host.
* **🧠 Heuristic Prompting**: Engineered specifically for `Llama 3.2`, providing structured outputs for competitive battle cards and email outreach without "hallucination noise."

---

## 🏗️ Technical Architecture



The tool uses a **Local Inference Loop**:
1.  **Frontend**: A standalone HTML/React file (Tailwind CSS for UI).
2.  **Bridge**: Fetch API calls directed to `http://localhost:11434/api/generate`.
3.  **Engine**: Ollama running as a background service, managing model weights and inference.

---

## ✨ Key Features

| Feature | Description |
| :--- | :--- |
| **🤖 100% Local AI** | Powered by Ollama; no data is ever uploaded to a third party. |
| **💰 Zero Costs** | No monthly subscription fees or token-based billing. |
| **🌐 Offline Mode** | Research and write emails on a plane or in remote areas—no internet required. |
| **🎯 Triple Threat** | Dedicated modules for **Company Research**, **Email Personalization**, and **Competitive Analysis**. |

---

## 🚀 Quick Start

### 1. Prerequisites
- **Ollama Installed** ([Download here](https://ollama.com))
- **8GB+ RAM** (Recommended for Llama 3.2)

### 2. Setup the Model
Open your terminal and run:
    ```bash
    ollama pull llama3.2

### 3. Launch the Tool
Download sales-tool.html.

Double-click to open in any modern browser.

Optional: To prevent CORS issues in some environments, serve via Python:
    ```bash
     python -m http.server 8000
Navigate to http://localhost:8000.

---

## 📊 Comparison: Local vs. Cloud AI

| Metric | Local Assistant | Commercial AI (SaaS) |
| :--- | :--- | :--- |
| **💰 Monthly Cost** | **$0 (Free)** | $20 - $600+ / month |
| **🔒 Data Privacy** | **100% Secure** (Stays on Disk) | Data processed on 3rd party servers |
| **🌐 Internet Required** | **No** (Works offline) | Yes (Always required) |
| **🛠️ Customization** | Full control over system prompts | Restricted by provider filters |
| **🚀 Speed** | Hardware dependent | Subject to server congestion |

---

## 📄 License
Distributed under the MIT License. 

Developed by [David Kok] – Private, powerful, and local sales enablement.

## ⭐ Love this tool? Give it a star on GitHub! ⭐
