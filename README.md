# DCL Evaluator

![Version](https://img.shields.io/badge/version-1.2.0-38bdf8?style=flat-square&logo=github)
![License](https://img.shields.io/badge/license-Source--Available-b8922a?style=flat-square)
![Patent](https://img.shields.io/badge/patent-pending-b8922a?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Windows-0078d4?style=flat-square&logo=windows)
![MCP](https://img.shields.io/badge/MCP-compatible-7dd3fc?style=flat-square)
![Offline](https://img.shields.io/badge/offline-capable-22c55e?style=flat-square)
![LLMs](https://img.shields.io/badge/LLMs-Claude%20%7C%20GPT--4%20%7C%20Grok%20%7C%20Gemini%20%7C%20Ollama-a78bfa?style=flat-square)

**Cryptographic audit trail for AI agents. Powered by Leibniz Layer™**

Every decision your AI agent makes — sealed, verified, auditable.

DCL Evaluator is the first implementation of [Leibniz Layer™](https://leibniz.fronesislabs.com) — a cryptographic verification protocol for AI agent decisions. It brings deterministic, tamper-evident audit trails to any LLM-powered system.

[![DCL Evaluator MCP server](https://glama.ai/mcp/servers/Fronesis-Labs/dcl-evaluator/badges/card.svg)](https://glama.ai/mcp/servers/Fronesis-Labs/dcl-evaluator)

---

## Why DCL Evaluator

AI agents make decisions. Those decisions carry risk — legal, financial, reputational. Yet most AI systems are black boxes: no record of what was decided, why, or whether the decision was tampered with afterward.

DCL Evaluator solves this with a simple principle borrowed from cryptography: **commit every decision into a hash chain**. Modify any past record and the entire chain invalidates. Mathematical proof of integrity — no trust required.

---

## Core capabilities

- **SHA-256 hash chain** — every agent action cryptographically sealed
- **Merkle tree audit trail** — tamper-evident by design
- **Deterministic policy engine** — identical input = identical decision, 100% reproducible
- **Drift detection** — statistical Z-test catches behavioural drift before it becomes a compliance failure
- **Multi-LLM support** — Claude, GPT-4, Grok, Gemini, DeepSeek, Ollama (local, air-gapped)
- **MCP server** — connect any agent in minutes via Model Context Protocol
- **Compliance reports** — tamper-evident PDF export, ready for regulators
- **Offline-capable** — runs fully air-gapped, zero data leaves your infrastructure

---

## Connect via MCP
```json
{
  "mcpServers": {
    "dcl-evaluator": {
      "url": "https://mcp.fronesislabs.com/sse",
      "headers": {
        "x-api-key": "your-key"
      }
    }
  }
}
```

Four tools available:

| Tool | Description |
|------|-------------|
| `dcl_commit` | Seal an agent action into the hash chain |
| `dcl_verify` | Verify chain integrity |
| `dcl_get_chain` | Retrieve full audit trail |
| `dcl_report` | Generate compliance report |

Health check: `https://mcp.fronesislabs.com/health`

---

## Download

→ [Latest release — v1.2.0](https://github.com/Fronesis-Labs/dcl-evaluator/releases)

Desktop app (Windows). Wails + Go + React. Works offline.

---

## Compliance coverage

Built-in policy templates:

`DEFAULT` · `EU AI ACT` · `GDPR` · `FINANCE` · `MEDICAL` · `RED TEAM`

---

## Leibniz Layer™

DCL Evaluator is the first product implementing **Leibniz Layer™** — the cryptographic verification layer for the AI agent economy.

Named after Gottfried Wilhelm Leibniz — mathematician, logician, pioneer of deterministic reasoning.

> *"Every decision, every action deterministically sealed, tamper-evident, auditable."*

[leibniz.fronesislabs.com](https://leibniz.fronesislabs.com)

---

## Links

- Website: [fronesislabs.com](https://fronesislabs.com)
- Leibniz Layer™: [leibniz.fronesislabs.com](https://leibniz.fronesislabs.com)
- IP & Patents: [leibniz.fronesislabs.com/ip-patents.html](https://leibniz.fronesislabs.com/ip-patents.html)
- MCP endpoint: [mcp.fronesislabs.com](https://mcp.fronesislabs.com/health)
- X: [@keykeeper42](https://x.com/keykeeper42)
- White Paper: [WHITEPAPER.md](./WHITEPAPER.md) · [leibniz.fronesislabs.com/whitepaper.html](https://leibniz.fronesislabs.com/whitepaper.html)

---

© 2026 Fronesis Labs · Leibniz Layer™, DCL Evaluator™ — Patent Pending · Source-Available License