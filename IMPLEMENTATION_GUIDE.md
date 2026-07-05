📡 Service Architecture Overview
Upon execution, the following services are initialized:

API Engine (FastAPI): Handles all agentic reasoning and command orchestration.
Telemetry Stream (WebSockets): Provides a low-latency bridge between the agent's "Thought Stream" and the React Dashboard.
Vector Store (ChromaDB): The persistence layer for long-term semantic memory.
Browser Instance (Playwright): A headless/headful Chromium instance controlled by the Sensory Layer.
