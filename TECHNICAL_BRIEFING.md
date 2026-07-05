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

---

## 🔬 Research & Development: Foundational Alignment

The Odysseus Framework is architected to address the current limitations identified in state-of-the-art (SOTA) Agentic Research. Our design principles are grounded in three primary domains of emerging AI science:

### 1. Hierarchical Task Decomposition (HTD)
While current LLM implementations often rely on flat, iterative loops, Odysseus implements a **Hierarchical Command & Control (C2) Model**. By applying **Hierarchical Multi-Agent Orchestration (H-MAO)**, the system can decompose complex, multi-modal objectives into specialized, stateful sub-tasks. This ensures high-fidelity execution by assigning "Worker" agents to specific operational niches (e.g., `WEB_SEARCH` vs. `CODE_AUDIT`) under the oversight of an Orchestration Layer.

### 2. Compute-Budgeted Adaptive Inference
A critical bottleneck in agentic autonomy is the competition for hardware resources (VRAM/GPU) during concurrent multimodal tasks. Odysseus addresses this through its **Dynamic VRAM Governor**. This implementation follows the principles of **Adaptive Resource Allocation**, where the agentic compute footprint scales in direct response to real-time system telemetry. This ensures that the agent maintains operational stability even when co-existing with high-load applications (e.g., UE5, 3D Rendering Engines).

### 3. Spatial-Semantic Mapping (S2A)
Odysseus moves beyond text-based interaction into the domain of **Spatial-Semantic Interaction**. By implementing a **Sensory-to-Action (S2A) Pipeline**, the framework maps digital/visual environments into a normalized coordinate-based intelligence layer. This allows for high-precision interaction within complex User Interfaces, bridging the gap between high-level linguistic intent and low-level, pixel-accurate execution.

---

---

## 📊 Visual Logic & Operational Flow

To visualize the transition from high-level intent to low-level execution, the Odysseus framework utilizes several adaptive workflow models. These models define how the agent allocates resources (VRAM/Compute) across different task lifecycles.

### **Adaptive Lifecycle Models**
*   **The Shipyard (Software Design):** A 4-stage logic flow focusing on architecture $\rightarrow$ deployment.
*   **The Studio Deck (Multimedia):** A 4-stage logic flow focusing on composition $\rightarrow$ mastering.
*   **The Foundry Line (Game Engineering):** A complex, high-resource loop involving 3D and audio dispatch.

*Detailed interactive diagrams can be found in the [Workflow Diagrams Hub](workflow_diagrams_index.html).*

---
*© 2026 Odysseus Framework. All Rights Reserved.*

graph TD
    subgraph Intelligence_Layer [🧠 Intelligence Layer: The Brain]
        A[User Command] --> B{Orchestrator}
        B --> C[Sub-Agent Spawning]
        C --> D[Semantic Memory/RAG]
        D --> B
    end

    subgraph Sensory_Layer [👁️ Sensory Layer: The Eyes & Hands]
        B --> E[Visual-Spatial Engine]
        B --> F[Browser Orchestrator]
        E --> G[Normalized Coordinates]
        F --> H[DOM Interaction]
        G --> I[Action Execution]
        H --> I
    end

    subgraph Interface_Layer [🎮 Interface Layer: Mission Control]
        I --> J[Telemetry Stream]
        J --> K[React Dashboard]
        K --> A
    end

    style Intelligence_Layer fill:#0c1a28,stroke:#38c6f5,stroke-width:2px,color:#e4f0ff
    style Sensory_Layer fill:#060c14,stroke:#3de898,stroke-width:2px,color:#e4f0ff
    style Interface_Layer fill:#0c1a28,stroke:#b080f8,stroke-width:2px,color:#e4f0ff


sequenceDiagram
    participant U as User / Architect
    participant O as Orchestrator
    participant S as Software Designer Agent
    participant E as Execution Environment

    U->>O: High-Level Architecture Request
    Note over O,S: [Stage 1: Keel Alignment]
    O->>S: Define Core System Structure
    S->>E: Scaffold Project (File Creation)
    
    Note over O,S: [Stage 2: Hull Framing]
    O->>S: Implement Core Logic & Interfaces
    S->>E: Write Module Implementations

    Note over O,S: [Stage 3: Systems Wiring]
    O->>S: Integrate Modules & Dependencies
    S->>E: Perform Automated Testing

    Note over O,S: [Stage 4: Launch Dock]
    O->>S: Final Validation & Deployment
    S->>E: Deploy to Runtime
    E-->>U: Deployment Successful

stateDiagram-v2
    [*] --> Idle
    Idle --> Monitoring: System Load Detected
    
    state Monitoring {
        [*] --> Low_Resource
        Low_Resource --> Medium_Resource: Compute Demand Increasing
        Medium_Resource --> High_Resource: Critical Demand (e.g. UE5 Active)
        High_Resource --> Low_Resource: Task Completed
    }

    state High_Resource {
        [*] --> TEXT_ONLY_MODE
        TEXT_ONLY_MODE --> AUDIO_GEN_MODE: Demand > Threshold
        AUDIO_GEN_MODE --> RENDER_3D_MODE: Critical Requirement
    }

    Monitoring --> Idle: Resource Threshold Reached
