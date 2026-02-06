# VeriForge Failure Taxonomy

VeriForge replaces the ambiguous concept of “hallucinations” with explicit failure categories.

Failure classification enables appropriate verification, escalation, and accountability.

---

## 1. Fabrication

**Definition:**  
The model generates facts, citations, or claims with no supporting evidence.

**Common causes:**  
- Over-generalization
- Pattern completion without grounding

**Mitigations:**  
- Fact verification
- Source validation
- Evidence-based certification

---

## 2. Miscommunication

**Definition:**  
The output is incorrect due to ambiguity or underspecification in the prompt.

**Examples:**  
- Pronoun ambiguity
- Implicit assumptions
- Unclear scope or intent

**Mitigations:**  
- Clarification request
- Pre-verification prompt refinement

---

## 3. Missing Data

**Definition:**  
Required information was unavailable or outside the model’s knowledge scope.

**Examples:**  
- Recent events
- Private or proprietary data

**Mitigations:**  
- Explicit abstention
- Qualified responses
- External data retrieval

---

## 4. Context Loss

**Definition:**  
Relevant constraints or prior information were dropped across turns.

**Examples:**  
- Long conversations
- State-dependent tasks

**Mitigations:**  
- Context reconstruction
- State verification
- Conversation replay

---

## 5. Over-generalization

**Definition:**  
The output is statistically plausible but operationally incorrect.

**Examples:**  
- Edge-case failures
- Domain-specific inaccuracies

**Mitigations:**  
- Domain-specific verifiers
- Constraint-based validation

---

## Notes

- Multiple failure types may co-occur
- Classification may be probabilistic
- Failure classification informs decision tier escalation
