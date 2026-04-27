<div align="center">

# Vercroww

**Policy-Gated Autonomous Escrow on Ethereum**

[![Next.js](https://img.shields.io/badge/Next.js-000?style=flat-square&logo=nextdotjs&logoColor=white)](https://nextjs.org)
[![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)](https://soliditylang.org)
[![Gemini](https://img.shields.io/badge/Gemini_AI-4285F4?style=flat-square&logo=google&logoColor=white)](https://ai.google.dev)

*Built at Blueprint 6.0 Hackathon*

</div>

---

## Concept

Traditional escrow requires trusted intermediaries — banks, lawyers, or platforms that charge fees and introduce delays. Vercroww replaces them with **AI-driven policy validation** and **smart contract automation**.

A buyer describes what they want in plain English. The AI parses the intent into structured conditions, validates them against predefined policies, and deploys a self-executing escrow contract on Ethereum.

---

## Architecture

```
Natural Language Intent
        │
        ▼
Intent Parser (Gemini 1.5 Flash)
   "Ship 500 units by March 15"  →  { type: delivery, qty: 500, deadline: "2026-03-15" }
        │
        ▼
Policy Validator
   Checks against configurable rules (max amount, allowed categories, etc.)
        │
        ▼
Smart Contract (Solidity)
   Deploys escrow on Sepolia testnet
   Funds locked → conditions met → auto-release
```

---

## What's Implemented

| Layer | Status |
|-------|--------|
| Intent parser — natural language to structured JSON | ✅ Working |
| Policy validator — rule-based condition checking | ✅ Working |
| Smart contracts — Sepolia testnet deployment | ✅ Deployed |
| Verification agents (delivery, quality) | 🔲 Simulated |
| Production blockchain (Arbitrum) | 🔲 Planned |

---

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Frontend | Next.js, Tailwind CSS |
| Smart Contracts | Solidity, Hardhat |
| AI | Google Gemini 1.5 Flash |
| Blockchain | Ethereum (Sepolia testnet) |
| Target L2 | Arbitrum (planned) |

---

## Context

This project was built during **Blueprint 6.0**, a 36-hour hackathon. The goal was to explore how AI can eliminate intermediaries in financial transactions by combining natural language understanding with programmable money.

The core innovation — parsing unstructured human intent into enforceable smart contract conditions — is functional. The verification and production deployment layers are scoped for future development.

---

## License

MIT

