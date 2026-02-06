# VeriForge Decision Tiers

VeriForge classifies AI decisions by **impact and reversibility**, not by model type or implementation.

The purpose of tiering is to ensure that verification effort is proportional to decision risk.

---

## Tier 3 — Neural models only

**Description:**  
Low-impact, easily reversible decisions.

**Examples:**  
- Drafting text
- Summarization
- Brainstorming
- Non-binding recommendations

**Controls:**  
- No external verification required

---

## Tier 2 — Neural + symbolic models

**Description:**  
Decisions requiring structured reasoning in constrained domains.

**Examples:**  
- Rule-based classification
- Policy checks
- Deterministic transformations

**Controls:**  
- Symbolic constraints
- Rule validation
- Consistency checks

---

## Tier 1 — Pre- and post-verification required

**Description:**  
High-impact decisions where incorrect outputs introduce material risk.

**Examples:**  
- Financial analysis
- Regulatory interpretation
- Safety-related recommendations

**Controls:**  
- Domain-specific verification
- Pre- or post-verification
- Certification artifacts

---

## Tier 0 — Human-in-the-loop required

**Description:**  
Irreversible decisions with legal, medical, or ethical consequences.

**Examples:**  
- Medical diagnosis
- Legal judgments
- Autonomous physical actions

**Controls:**  
- Human approval
- Explicit accountability
- Recorded justification

---

## Notes

- Tiering may change dynamically based on context
- Escalation between tiers is expected
- Tier boundaries are intentionally conservative
