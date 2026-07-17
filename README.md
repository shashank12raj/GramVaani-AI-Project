# GramVaani AI Project

An advanced, conversational AI assistant designed to streamline communication and deliver intelligent, context-aware automated responses. This project leverages visual orchestrations via Flowise and state-of-the-art LLM processing with Google Gemini.

---

## Live Links
* "Click Here for Live Demo:" [https://cloud.flowiseai.com/chatbot/89920d49-5023-4fe3-86cb-9d7f6e6cc593] 
* "Live Deployment:" [https://flowise-ai-production-e53f.up.railway.app/chatbot/c0aa046d-da78-46c6-a571-620702ba285c] -The free valid period is of 30 days only, it will not work after 16th july 2026.
* "Orchestration Server:" Hosted live on Railway "30 days free period"

---

## 🛠️ Tech Stack & Architecture

This application utilizes a modular, low-code AI infrastructure to handle active conversational logic seamlessly:

* **Orchestration Layer:** Built visually inside **Flowise AI**, enabling custom memory retention and smooth conversational chaining.
* **Core Intelligence (LLM):** Powered by the **Google Gemini (gemini-2.5-flash)** API for ultra-fast, responsive natural language processing.
* **Memory Management:** Features a **Buffer Memory** block node to track ongoing conversation states and recall historical message contexts.
* **Hosting Platform:** Deployed dynamically in the cloud using **Railway** with persistent database volume storage.

---

## 📊 Visual Workflow Diagram

The system architecture flows as follows:

1. **User Input:** Message is passed directly via the public web-chat interface.
2. **Contextual Retrieval:** The **Conversation Chain** queries the **Buffer Memory** to extract active conversation history.
3. **Model Processing:** The historical context and new prompt are packaged and fed directly into the **Google Gemini** node.
4. **Output Response:** The model delivers a natural language string back to the user interface while simultaneously writing the turn to memory.

---

## 📂 How to Import & Run Locally / in Cloud

If you wish to clone this setup or import it into your own Flowise instance:

1. Set up a fresh instance of **Flowise AI** (locally via npm or hosted on platforms like Railway).
2. Create a blank chatflow workspace canvas.
3. Click on the workspace settings gear icon, select **Load Chatflow**, and upload the `GramVaani...json` file found in this repository.
4. Open the **Google Gemini** credential configuration block inside your canvas and insert your unique **Google AI Studio API Key**.
5. Click **Save** to deploy the agent.
