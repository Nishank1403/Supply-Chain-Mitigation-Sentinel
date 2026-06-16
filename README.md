Supply Chain Sentinel 
🛡️📦Supply Chain Sentinel is an autonomous AI agent designed to monitor, triage, and automatically 
optimize supply chain operations by detecting anomalies and orchestrating resolutions in real-time. 
This project was built and submitted for the Microsoft Agents League Hackathon (AI Skills Fest 2026).

🚀 Project OverviewThe core objective of Supply Chain Sentinel is to eliminate operational downtime and 
minimize supply chain risks through automated governance. By combining generative AI orchestration with 
automated workflows, the system detects disruptions (e.g., shipment delays, stock shortages, or logistical 
anomalies) and executes remediation paths without requiring constant human intervention.
Core Key Features
Autonomous Anomaly Detection: Real-time evaluation of data streams to flag supply chain deviations.
Intelligent Escalation & Triage: Automated impact assessment and risk classification.
Automated Procurement Dispatch: Dynamic creation and routing of remediation orders.
Comprehensive Audit Logging: Transparent tracking of every agentic decision and automated flow execution.

🏗️ Structural ArchitectureThe solution relies entirely on the Microsoft AI and Power Platform ecosystem 
to provide a robust, low-latency, and secure enterprise workflow:
[ User / Data Stream ] 
       │
       ▼
┌─────────────────────────────────┐
│  Microsoft Copilot Studio Agent │ <── Primary Interaction & Reasoning Hub
└────────────────┬────────────────┘
                 │
                 ▼
┌─────────────────────────────────┐
│      Power Automate Flows       │ <── Business Logic & Action Execution
└────────────────┬────────────────┘
                 │
                 ▼
┌─────────────────────────────────┐
│   Microsoft Fabric Integration  │ <── Unified Data Lakehouse & Analytics
└─────────────────────────────────┘
Microsoft Copilot Studio Agent: Acts as the central reasoning engine that interacts with stakeholders, 
interprets supply chain anomalies, and coordinates background system tasks.
Power Automate Flows: Handles the complex event-driven architecture, triggering multi-step integrations 
across procurement and communication channels when an incident occurs.
Microsoft Fabric Integration: Serves as the central data repository, storing analytics, current supply 
chain states, and historical baseline data for rapid telemetry ingestion.
📁 Repository Structure
files├── ExecuteSupplyChainMitigation_20260609014642.zip  # Packaged Power Automate flow solutions
├── HandleSupplyChainGovernanceExecution_20260609014719.zip # Copilot governance workflows
└── Technical_Walkthrough.pdf                        # Project documentation and architectural details
Use code with caution.
📺 Video Walkthrough GuideThe repository includes a complete demonstration of the system in action. 
Refer to the timestamp guide below inside your video submission:00:00 - 00:15 | Environment Overview: Initial tour of the Copilot Studio workspace and Microsoft Fabric pipeline setups.00:15 - 00:30 | Flow Automation Framework: Deep dive into the underlying Power Automate infrastructure connecting the modules.00:30 - 00:45 | Simulating an Anomaly: Triggering an artificial logistical block or material shortage to test system awareness.00:45 - 01:00 | Automated Triage Run: The Copilot agent intercepting the event, assessing risks, and evaluating resolution vectors.01:00 - 01:15 | Procurement Dispatch: Execution of automatic vendor outreach or purchase order revisions to remedy the shortage.01:15 - 01:30 | Resolution and Audit Logs: Final resolution verification and logging of telemetry states inside Microsoft Fabric.🛠️ Installation & SetupTo import and inspect the solution packages locally:Prerequisites: Ensure you have active access to a Power Apps / Power Automate environment with Premium connectors enabled, as well as a Microsoft Fabric capacity tenant.Import Flows: Navigate to Power Automate, click Import > Legacy Package, and upload the ExecuteSupplyChainMitigation and HandleSupplyChainGovernanceExecution zip solutions.Configure Copilot Studio: Import the target bots using the package components inside Microsoft Copilot Studio.Connect Data Source: Repair and authenticate the environment connections pointing to your Microsoft Fabric workspace tables.If you need any adjustments to the architecture wording or want to add explicit instructions for environment variables, let me know!
