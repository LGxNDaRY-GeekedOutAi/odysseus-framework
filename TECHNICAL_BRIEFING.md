# 🌌 Odysseus: Technical Briefing
### *Architecture & Orchestration Logic for Multi-Agentic Systems*

**Version:** 0.0.92  
**Status:** Technical Overview (Public-Facing)  
**Subject:** Adaptive Multi-Agentic Orchestration & Resource Governance

---

## 🔭 Executive Summary
The **Odysseus Framework** is a high-performance Command & Control (C2) orchestration engine. Unlike standard LLM wrappers, Odysseus utilizes a **Triple-Layer Architecture** designed to manage the lifecycle of complex digital tasks by balancing cognitive reasoning with hardware-aware resource constraints.

The framework is built to solve the "Agentic Resource Exhaustion" problem: ensuring that autonomous agents can execute intensive multimodal workflows without destabilizing the host system's primary compute resources.

---

## 🏗️ The Triple-Layer Architecture

### 1. 🧠 The Intelligence Layer (Cognitive Orchestration)
The core of Odysseus is a stateful agentic loop built on **FastAPI**. It manages task hierarchies through a sophisticated "Persona Orchestration" system.
*   **Semantic Memory (RAG):** Leveraging **ChromaDB** and **Sentence-Transformers**, the system implements long-term cognitive persistence, allowing agents to maintain context, preferences, and historical decision-making patterns across sessions.
*   **Stateful Orchestration:** The engine manages sub-agent spawning, maintaining a persistent "Thought Stream" that tracks the progression from intent to execution.

### 2. 👁️ The Sensory Layer (Perception & Action)
The Sensory Layer converts raw digital environments into actionable intelligence through two primary pipelines:
*   **Visual-Spatial Pipeline:** A multimodal vision-to-coordinate engine that maps visual UI elements into a normalized coordinate system, enabling high-precision interaction in browser and desktop environments.
*   **Browser/System Orchestration:** Leveraging **Playwright**, the agent operates within live environments, performing human-like navigation, data extraction, and complex UI interaction.

### 3. 🎮 The Interface Layer (Telemetry & Command)
The user interacts via a high-performance **React/Vite** dashboard designed for "Zen-mode" efficiency.
*   **Real-time Telemetry:** The interface provides a live stream of agentic "thought processes," command execution, and system vital signs (token velocity, latency, and compute load).
*   **Modular Command:** A minimalist interface that expands into a full "Mission Control" dashboard during active high-intensity operations.

---

## ⚖️ Hardware-Aware Resource Governance (VRAM Governor)

A distinguishing feature of Odysseus is its **Dynamic VRAM Governance**. Recognizing that multi-agentic tasks often compete for GPU resources, Odysseus implements a 10-tier resource classification system:

| Tier | Classification | Primary Modality | Compute Profile |
| :--- | :--- | :--- | :--- |
| **T1** | **TEXT_ONLY** | Text/Code | Low-VRAM / High-Speed |
| **T2** | **AUDIO_GEN** | Music/Voice | Moderate VRAM |
| **T3** | **IMAGE_GEN** | 2D Assets | High VRAM |
| **T4** | **VIDEO/3D** | Motion/Render | Critical VRAM |

The **VRAM Governor** dynamically adjusts the agent's operational mode based on active system requirements (e.g., monitoring real-time usage of high-load applications like `UE5Editor.exe`). This ensures that the agent's resource footprint scales inversely to the host's immediate computational demands.

---

## 🔄 Adaptive Workflow Modes
Odysseus utilizes **Adaptive Lifecycle Stages** to transition from high-level intent to granular execution. Depending on the active profile, the system moves through specialized stages:

*   **Design/Architect Modes:** Focus on structured logic (e.g., *Keel Alignment $\rightarrow$ Hull Framing $\rightarrow$ Launch Dock*).
*   **Creative/Multimedia Modes:** Focus on asset generation and media dispatch (e.g., *Score Brief $\rightarrow$ Theme Forge $\rightarrow$ Mix Master*).
*   **Engineering/Technical Modes:** Focus on rapid iteration and code auditing with strict adherence to policy-gated execution.

---

## 🛠️ Technical Stack Summary
*   **Backend:** Python, FastAPI, Uvicorn
*   **Frontend:** React, Vite, Tailwind CSS, Framer Motion
*   **Vector/Memory:** ChromaDB, Sentence-Transformers
*   **Automation:** Playwright (Chromium)
*   **Orchestration:** Multi-Agentic State Machine

---
*© 2026 Odysseus Multi-Agentic Framework. All Rights Reserved.*
