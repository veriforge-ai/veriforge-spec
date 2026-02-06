# VeriForge

**VeriForge** is an open framework and protocol for **verified AI decisions**.

As AI systems move from assistance to autonomy, accuracy alone is insufficient. Real-world systems require **verified outcomes** — outcomes that can be audited, insured, and assigned responsibility.

VeriForge defines **when, how, and where** AI systems should invoke verification before an output is relied upon.

---

## What VeriForge Is

VeriForge is:
- A **decision-verification framework**
- A **protocol** for invoking and recording verification
- A **shared taxonomy** for decision tiers and failure modes
- An **ecosystem** for verification tools, experts, and services

VeriForge is **model-agnostic**. It applies equally to:
- Dense neural models
- Mixture-of-Experts architectures
- Symbolic systems
- Hybrid or agentic systems

---

## Why VeriForge Exists

Improving model accuracy reduces error rates, but it does not establish responsibility.

The real world operates on **verified results**:
- Decisions that can be audited
- Outcomes that can be insured
- Processes that demonstrate due diligence

Without verification:
- Liability is undefined
- Risk cannot be transferred
- Responsibility is unclear

VeriForge exists to make verification a **first-class capability** in AI systems.

---

## Core Concepts

### 1. Decision Tiering

Not all AI decisions require the same level of scrutiny. VeriForge classifies decisions by **impact and reversibility**, not by model type.

- **Tier 3 — Neural models only**  
  Low-impact, reversible decisions

- **Tier 2 — Neural + symbolic models**  
  Structured reasoning in constrained domains

- **Tier 1 — Pre- and post-verification required**  
  High-impact, regulated, or safety-relevant decisions

- **Tier 0 — Human-in-the-loop required**  
  Irreversible legal, medical, or ethical decisions

---

### 2. Failure Classification (Beyond “Hallucinations”)

The term *hallucination* is an imprecise catch-all. VeriForge replaces it with explicit failure categories, including:

- **Fabrication** — unsupported facts were invented
- **Miscommunication** — ambiguity in prompts (pronouns, scope, intent)
- **Missing data** — required information was unavailable
- **Context loss** — constraints dropped across turns
- **Over-generalization** — statistically plausible, operationally wrong

Different failures imply different verification strategies.

---

### 3. Verification Protocol

At a minimum, a VeriForge-compliant system performs the following steps:

1. An output is produced
2. The decision tier is determined
3. Appropriate verifier(s) are selected
4. The output is evaluated against domain and risk constraints
5. A certification, qualification, or rejection is issued
6. Verification evidence is recorded

Verification may occur **before or after** an answer is generated. In some cases, the primary interaction is verification rather than generation.

---

## Implementation Approach

VeriForge is designed to be implemented **on top of MCP-compatible gateways**.

Existing gateways — such as **ContextForge** — can serve as execution engines for VeriForge verification workflows. In this model:

- The gateway handles routing and orchestration
- VeriForge defines verification semantics, controls, and certification requirements
- Verification tools and experts are exposed as callable services

This separation allows multiple independent implementations while preserving consistent verification behavior.

---

## What VeriForge Is Not

VeriForge is not:
- A new model architecture
- A replacement for performance optimizations such as Mixture-of-Experts
- A reasoning engine or inference system
- Another MCP Server Gateway

VeriForge complements advances in model architecture by providing **governance, assurance, and accountability**.

---

## Status

VeriForge is in an early, exploratory stage.

Feedback, critique, and real-world pressure testing are explicitly encouraged.

---

## License

VeriForge is licensed under the **Apache License 2.0**.
