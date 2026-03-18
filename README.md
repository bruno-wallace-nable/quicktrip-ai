# ✈️ QuickTrip AI

An AI-powered travel planner built with Ruby on Rails that generates personalized itineraries through a real-time chat experience.

QuickTrip AI allows users to create trips and interact with an AI assistant that dynamically generates travel plans using streaming responses and background processing.

🔗 Live Demo: https://quicktrip-ai-53d7a1d73f9b.herokuapp.com/

---

## 🚀 Overview

Planning a trip can be time-consuming and overwhelming. QuickTrip AI simplifies this process by combining artificial intelligence with a smooth, real-time chat interface.

Users can create a trip, describe their preferences, and receive a personalized itinerary generated asynchronously, with responses streamed directly into the interface.

This project was designed to simulate a real-world SaaS product, focusing on performance, user experience, and scalable architecture.

---

## ✨ Features

- 🤖 AI-generated travel itineraries
- 💬 Real-time chat interface
- ⚡ Streaming responses (Turbo Streams)
- 🔄 Asynchronous processing with background jobs
- 🧠 Context-aware AI prompts
- 🔐 User authentication
- 🗂️ Trip history and persistence
- 📱 Responsive UI

---

## 🛠 Tech Stack

**Backend**
- Ruby on Rails
- PostgreSQL / SQLite
- Active Job

**Frontend**
- Turbo (Hotwire)
- Stimulus.js
- HTML / CSS

**Real-time**
- ActionCable (WebSockets)
- Turbo Streams

**AI Integration**
- OpenAI API

**Deployment**
- Heroku

---

## 🧱 Architecture

The application follows a standard Rails MVC structure enhanced with real-time and asynchronous capabilities:

- **Turbo Streams** handle real-time UI updates
- **ActionCable** enables WebSocket-based communication
- **Background jobs** process AI responses without blocking the UI
- **Stimulus controllers** manage frontend interactivity

This architecture allows the app to deliver a smooth, responsive chat experience while handling potentially slow AI responses in the background.

---

## ⚙️ How It Works

1. The user creates a new trip
2. A chat session is initialized
3. The user sends a message describing the desired itinerary
4. A background job sends the request to the AI
5. The AI response is processed asynchronously
6. The response is streamed back into the chat interface in real time

---

## 🧪 Setup Instructions

### Clone the repository

```bash
git clone https://github.com/robertodefarias/quicktrip-ai.git
cd quicktrip-ai
