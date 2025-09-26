---
description: >-
  Hyperrun.ai is powered by a lightweight, modular infrastructure designed for
  conversational trading.
icon: message-bot
---

# How Hyperrun Works

#### Context Sources

* Real-time Hyperliquid market data
* Your wallet history (balances, trades, performance)
* Cross-chain bridging activity
* User inputs (chat prompts, voice commands, strategy rules)

#### Core Engine

* **Vector Storage** → Stores context and makes it retrievable for your agent.
* **Active Functions** →
  * Spot & perp execution
  * Bridging operations
  * Strategy simulation and backtesting
* **Output Composer** → Converts complex workflows into clear, natural responses.

#### Example Workflow

1. You say: “Open a 5x BTC long with $200 if funding rates are below 0.01%.”
2. The system:
   * Checks funding rates
   * Calculates slippage + risk
   * Executes the order if conditions are met
3. You get a clear confirmation in plain natural language.
