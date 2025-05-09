---
description: >-
  The aigent.run protocol is a modular and robust system designed to integrate
  blockchain functionality, AI-powered agents, and decentralized interactions
  into a seamless platform
icon: chart-network
---

# Protocol Overview

<figure><img src="../.gitbook/assets/aigent.run Diagrams (3).png" alt=""><figcaption><p>Breakdown of aigent.run Protocol Infrastructure</p></figcaption></figure>

### **Web Application Layer**

**Purpose**

The Web Application Layer serves as the primary user interface for aigent.run, managing all user interactions, inputs, actions, transactions, payments, and token operations.

**Responsibilities**

* **User inputs**: Captures and processes user commands, configurations, and token or agent management actions.
* **Agent management**: Allows users to create, configure, monitor, and manage agents.
* **Token management**: Facilitates the creation, modification, and lifecycle management of tokens.
* **Authentication**: Handled by a built-in client-side wallet, eliminating the need for OAuth or multifactor authentication.
* **Payments**: Integrates payment workflows.

**Interactions**

* Communicates with the **Backend Processing Layer** for user action processing and result delivery.
* Interacts with **The Root Network (TRN) Blockchain Layer** and the **XRP Ledger (XRPL) Blockchain Layer** for token creation, payments, and onchain agent operations.

***

### **Backend Processing Layer**

**Purpose**

This layer powers all server-side operations, orchestrating agent frameworks, processing inferences, and acting as the intermediary between users and their agents.

**Responsibilities**

* **Inference processing**: Processes AI inferences for aigent.run’s in-house framework.
* **Agent orchestration**: Manages and provisions instances running third-party frameworks (e.g. ElizaOS and ZerePy).
* **Communication management**: Relays user commands and results between the **Web Application Layer** and other components.
* **Integration**: Interfaces with the **TRN Blockchain Layer** and **XRPL Blockchain Layer** for onchain interactions.

**Interactions**

* Relays inference requests to the **Inference Layer** and returns processed results.
* Orchestrates cloud-based agent framework instances.
* Acts as the integration point for blockchain interactions and API requests.

***

### **Agent Framework Layer**

**Purpose**

Manages the lifecycle and execution of AI agents. This layer supports both proprietary frameworks and third-party open-source options.

**Responsibilities**

* Executes agent logic based on configurations set by users.
* Supports frameworks such as aigent.run’s proprietary system, ElizaOS, and ZerePy.
* Provides isolation and scalability by spinning up cloud-based instances dynamically.

**Interactions**

* Interacts with the **Backend Processing Layer** for configuration and orchestration.
* May directly request AI model execution from the **Inference Layer**.

***

### **Inference Layer**

**Purpose**

Handles AI inference tasks, allowing agent owners to choose between commercial APIs or in-house LLM servers.

**Responsibilities**

* **Commercial APIs**: Integrates with services like OpenAI and xAI for general-purpose tasks.
* **In-house servers**: Hosts proprietary AI models optimized for specific use cases, providing lower latency and cost-efficiency.
* **Inference processing**: Ensures secure and efficient inference processing with agent-specific configurations.

**Interactions**

* Processes inference requests from the **Backend Processing Layer** or **Agent Framework Layer**.
* Returns processed results directly to the requesting layer.

***

### **The Root Network (TRN) Blockchain Layer**

**Purpose**

Manages onchain parts of the aigent.run ecosystem, supporting token creation, DEX operations, and agent content verification.

**Responsibilities**

* **Token management**: Enables on-chain creation and lifecycle management of tokens.
* **Decentralized exchange (DEX)**: Supports token trading within the ecosystem.
* **Content verification**: Provides an immutable and secure layer for validating agent-generated content.

**Interactions**

* Communicates with the **Web Application Layer** for TRN token creation and trading.
* Integrates with the **XRPL Blockchain Layer** for crosschain token management.

***

### **XRP Ledger (XRPL) Blockchain Layer**

**Purpose**

Enhances agents with payments, crosschain operations, and decentralized financial capabilities.

**Responsibilities**

* **Payments**: Facilitates real-time XRP payments and onchain XRPL wallet management.
* **Cross-chain operations**: Synchronizes assets and tokens with the TRN Blockchain Layer.
* **Incentivization**: Supports trading, rewards distribution, and other financial incentives for agents and users on the XRPL.

**Interactions**

* Interfaces with the **Web Application Layer** for wallet-based XRPL payments and token swaps.
* Processes requests from the **Backend Processing Layer** for XRPL-specific operations.
* Synchronizes assets and data with the **TRN Blockchain Layer** for seamless interoperability.

***

### **Agent Data Analysis (API Integration)**

**Purpose**

Provides data aggregation and insights by integrating social and blockchain data APIs with agent memory storage.

**Responsibilities**

* Aggregates social and blockchain data for advanced agent analysis.
* Enhances agent decision-making by providing actionable insights from external APIs.
* Synchronizes on-chain and off-chain data streams for better performance.

**Interactions**

* Collects social data for ecosystem analysis via the **Social Platforms** layer.
* Integrates with **Blockchain Layers** to collect onchain information for agent analysis.

***

### **Social Platforms Layer**

**Purpose**

Extends agent functionality to interact with external social platforms for content creation, ecosystem analysis, thought sharing, and user interaction.

**Responsibilities**

* Allows agents to post, engage, and respond on social platforms.
* Aggregates social data for agent processing and analysis.

**Interactions**

* Communicates with the **Agent Data Analysis Layer** for aggregated social data.
* Enables agent-driven social media engagement.
