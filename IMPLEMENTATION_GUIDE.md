📡 Service Architecture Overview
Upon execution, the following services are initialized:

API Engine (FastAPI): Handles all agentic reasoning and command orchestration.
Telemetry Stream (WebSockets): Provides a low-latency bridge between the agent's "Thought Stream" and the React Dashboard.
Vector Store (ChromaDB): The persistence layer for long-term semantic memory.
Browser Instance (Playwright): A headless/headful Chromium instance controlled by the Sensory Layer.

---

## 🛠️ The Skill Registry (Capability Catalog)

The Odysseus framework operates through a modular "Skill" architecture. Instead of a monolithic agent, Odysseus utilizes a **Skill Registry** that allows the Orchestration Layer to dynamically load and execute specific capabilities based on the current mission profile.

### **1. Core Operational Skills (Universal)**
These skills are available across all operational profiles:

| Skill ID | Capability Name | Description | Interaction Mode |
| :--- | :--- | :--- | :--- |
| `web_research` | **Deep Web Intelligence** | Multi-source browsing, data scraping, and synthesis of real-time web information. | Browser/DOM |
| `file_ops` | **FileSystem Management** | Read, write, move, and organize files within the authorized workspace. | Local Shell |
| `code_exec` | **Sandboxed Code Execution** | Safe execution of Python/Node.js code for complex mathematical or data processing tasks. | Python/Kernel |
| `thought_log` | **Cognitive Telemetry** | The ability to write "Chain-of-Thought" (CoT) reasoning to the telemetry stream. | Internal/Stream |

### **2. Specialized Agentic Skills (Profile-Dependent)**
These skills are dynamically injected into the agent's context based on the active **Mission Profile**:

#### **A. Software Designer Profile (Shipyard Mode)**
*   `git_flow`: Managing branch creation, commits, and pull requests.
*   `syntax_audit`: Running static analysis and linting on code blocks.
*   `dep_check`: Verifying package dependencies and version compatibility.

#### **B. Music Composer Profile (Studio Deck Mode)**
*   `audio_gen`: Triggering local/API-based generative audio models.
*   `waveform_inspect`: Analyzing audio metadata and frequency profiles.
*   `asset_export`: Managing the transition from MIDI/Code to high-fidelity audio files.

#### **C. Game Designer Profile (Foundry Line Mode)**
*   `ue5_sync`: Monitoring real-time UE5 Editor state and VRAM consumption.
*   `asset_dispatch`: Pushing 3D/Audio/Texture assets into specific project directories.
*   `log_monitor`: Watching real-time engine logs for runtime errors.

### **3. Sensory-to-Action (S2A) Interface**
The ultimate skill set in the Odysseus ecosystem is the **S2A Capability**, which allows the agent to bridge the gap between "Thinking" and "Doing" in a visual environment:

*   **`visual_inspect`**: Translating raw pixels/screenshots into semantic object descriptions.
*   **`coordinate_click`**: Executing mouse/keyboard actions at normalized screen coordinates.
*   **`dom_query`**: Direct interaction with the browser's Document Object Model for precision UI automation.

---

*© 2026 Odysseus Multi-Agentic Framework. All Rights Reserved.*
