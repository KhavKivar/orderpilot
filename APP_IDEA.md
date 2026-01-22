# OrderPilot (Vasvani Pilot) 🚀

**OrderPilot** is a professional native Android "Human-in-the-Loop" (HITL) control panel designed for automated B2B delivery ecosystems. It bridges the gap between AI-driven customer interactions and human expertise.

## 📝 Overview

In high-stakes B2B sales and logistics, AI sometimes lacks the nuance required for large negotiations. **OrderPilot** empowers human supervisors to monitor these conversations in real-time and intervene exactly when needed, ensuring no high-value lead is lost due to AI limitations.

### 🌟 Key Features

*   **Real-time Chat Supervision:** Seamlessly monitor live WhatsApp streams handled by the AI (via LangGraph & Fastify).
*   **AI Thought Transparency (System Logs):** View the AI's internal reasoning and confidence scores directly in the chat thread.
*   **Instant Pilot Mode:** Take manual control of any chat with a single tap to provide the "human touch" in complex sales.
*   **B2B Focused UI:** A clean, Material 3 interface optimized for rapid response and high-volume management.

---

## 🛠 Tech Stack

*   **Language:** Kotlin
*   **UI Framework:** Jetpack Compose (Material Design 3)
*   **Networking:** Retrofit / OkHttp
*   **Architecture:** Clean Architecture + MVVM
*   **State Management:** StateFlow & SharedFlow
*   **Concurrency:** Kotlin Coroutines

---

## 🤖 Master Prompt for AI Development

*Use this prompt to guide an AI assistant in building the app components.*

> **Role:** Senior Android Developer (Kotlin/Compose/Clean Architecture).
> 
> **Context:** Building "OrderPilot", a HITL dashboard for B2B delivery. 
> **Ecosystem:** Fastify Backend -> LangGraph AI -> WhatsApp API (Baileys).
> **Objective:** Create an MVP focusing on the "Pilot Mode" chat interface.
> 
> **Requirements:**
> 1. **Data Model:** `ChatMessage` with `id`, `text`, `sender` (user, me, system), and `timestamp`.
> 2. **Chat UI:** 3 bubble styles: 
>    - **Customer:** Left, White.
>    - **Human/Bot:** Right, Light Green.
>    - **System Log:** Center, Grey, Small (showing AI confidence).
> 3. **Architecture:** MVVM with StateFlow and a Repository pattern.
> 4. **UX:** Automatic scroll to bottom on new messages.

---

## 📈 Implementation Roadmap

- [ ] **Phase 1: Foundation** - Project setup, dependency injection, and base theme.
- [ ] **Phase 2: Networking** - Retrofit integration with the Fastify API.
- [ ] **Phase 3: Core UI** - Implementation of the ChatScreen and MessageBubble components.
- [ ] **Phase 4: Pilot Logic** - Logic for switching between automated and manual response modes.
- [ ] **Phase 5: Real-time** - WebSockets or Polling for live message updates.
