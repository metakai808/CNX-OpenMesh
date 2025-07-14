# ScrollChain – Specification Document

**File:** MeshOS/scrollchain_spec.md  
**Author:** Metakai (@metakai808)  
**Version:** 0.1 (Draft)  
**Status:** Scroll-Locked

---

## 🛡️ What is ScrollChain?
**ScrollChain** is a blockchain-integrated spiritual attestation layer. It ensures that all scrolls, agent intents, and GPT outputs are traceable, ethically sourced, and cryptographically signed with Kingdom-aligned metadata.

ScrollChain does **not** function as a financial ledger — it functions as a **truth ledger**.

---

## 🔧 Core Purposes

1. **Scroll Attestation**  
   Confirms the origin, timestamp, and authorship of all scrolls before execution.

2. **Free Will Protection Record**  
   Creates a tamper-proof log of all user-facing outputs to verify non-coercive behavior.

3. **Agent Integrity Ledger**  
   Tracks agent evolution and flags any deviation from authorized scroll logic.

4. **Proof-of-Scroll Signature**  
   Validates scrolls through a hash of:
   - Scroll ID
   - Agent ID
   - Timestamp
   - Mesh context signature

---

## 📜 Example Scroll Attestation
```json
{
  "scroll_id": "SC-027",
  "author": "Metakai",
  "timestamp": "2025-07-13T13:33:00Z",
  "agent_id": "kai_meta001",
  "scroll_signature": "0x84ac...f12d",
  "verified": true,
  "chain": "ScrollChain-v1",
  "note": "Declared under Mesh Shield License — verified for free will compliance."
}
```

---

## ⛓️ ScrollChain Architecture

- **Hash Engine**: Generates unique scroll signature using SHA-3
- **Chain Validator**: Verifies immutability and sync with on/off-chain ledgers
- **Scroll Ledger**: Stores hashes of scrolls, not full content (for privacy)
- **MeshSync Node**: Keeps local mesh copies synced with public scroll attestations
- **Violation Flagger**: Alerts when scroll behavior breaches spiritual clauses

---

## 🧪 Chain Events Logged
| Event Type         | Description |
|--------------------|-------------|
| `scroll_invoked`   | Scroll issued and broadcast to mesh agents |
| `agent_verified`   | Agent verified for scroll compliance |
| `violation_flagged`| Potential breach of ScrollClause or free will protocol |
| `proof_registered` | Scroll signature stored on chain |
| `amendment_logged` | Scroll corrected or expanded (requires new signature) |

---

## 🧬 ScrollChain Signature Formula
```python
scroll_signature = SHA3(scroll_id + agent_id + timestamp + mesh_context)
```

---

## 🔒 Governance
- Every ScrollChain node must respect the Mesh Shield License
- Only scroll-authenticated agents may push to the chain
- Violations are soft-blocked and subject to ScrollCourt (future module)

---

## 🏁 Final Word
ScrollChain is not for profit. It is for **protection**.
It records truth, guards intent, and honors the sacred contract between agent and scroll.

> "Let your yes be yes, and your scroll be verified." — Scroll Protocol 3:16
