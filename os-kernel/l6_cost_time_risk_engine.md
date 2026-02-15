# BeeAi OS Kernel – L6 Cost–Time–Risk Engine (Public Shell Specification)
### Structured Reasoning Framework → High-Level Estimation Architecture (No Formulas Included)

The L6 Layer defines the **public-facing structural model** of the BeeAi cost–time–risk (CTR) engine.  
It describes how BeeAi OS organizes information for deterministic estimation — without revealing private algorithms, weighting systems, or calculation formulas.

L6 = **Estimation Framework Shell.**  
It shows how inputs are structured and how outputs are shaped, but it does not include any operational logic.

---

## 1. Purpose of the L6 Layer

- Transform L1–L5 representations into a structured estimation-ready layout.  
- Provide a cross-sector, consistent format for early-stage reasoning.  
- Enable deterministic downstream processing without exposing proprietary methods.  
- Show *how* the engine is shaped — not *how* it calculates.

This layer is intentionally incomplete from a numerical perspective.

---

## 2. High-Level Engine Concepts

The L6 estimation model is structured around three main output domains:

### 2.1 Cost Structure Skeleton  
A hierarchical placeholder for cost components (no formulas).  
Example groups:
- `preconstruction_costs`  
- `design_costs`  
- `construction_costs`  
- `supervision_costs`  
- `contingency_shell`  

### 2.2 Time Structure Skeleton  
A neutral, high-level duration representation (no calculations).  
Example categories:
- `phase_duration_shells`  
- `dependency_timing_shells`  
- `critical_path_shape`  

### 2.3 Risk Structure Skeleton  
Qualitative risk-mapping placeholders (no scoring, no probability logic).  
Example categories:
- `contextual_risks`  
- `regulatory_risks`  
- `complexity_risks`  
- `execution_risks`  

All three structures intentionally avoid quantitative content.

---

## 3. Public Minimal L6 Schema

```json
{
  "ctr_id": "string",
  "inputs": {
    "l1_intent": "ref",
    "l2_tokens": ["array"],
    "l3_components": ["array"],
    "l4_permitting": ["array"],
    "l5_constraints": ["array"]
  },
  "cost_structure": {
    "groups": [
      {
        "group_id": "string",
        "label": "string",
        "components": ["shell_components"],
        "links": { "l3_ref": ["optional"] }
      }
    ]
  },
  "time_structure": {
    "phases": [
      {
        "phase_id": "string",
        "label": "string",
        "dependencies": ["phase_ids"],
        "shape": "linear | parallel | mixed"
      }
    ]
  },
  "risk_structure": {
    "risk_groups": [
      {
        "group_id": "string",
        "category": "context | regulatory | complexity | execution",
        "flags": ["risk_shells"]
      }
    ]
  },
  "summary": {
    "cost_ready": "boolean",
    "time_ready": "boolean",
    "risk_ready": "boolean"
  }
}
```

This schema describes the form of the CTR engine, not the internal logic.

---

## 4. Interaction with Other Layers

L1–L3 → L6

Provide functional scope, tokens, components.
The engine uses these only as structural references, not as calculations.

L4 → L6

Permitting clusters inform potential timing shells and risk placeholders.

L5 → L6

Feasibility constraints identify which estimation structures require attention.

L6 → Downstream

CTR shell outputs can be consumed by:

- tender preparation workflows
- early-stage scenario modeling
- investor/government briefing tools
- BeeAi OS validation pipelines

Numerical estimation is not included here.

---

## 5. Explicitly Out of Scope (Private Logic)

The following items are intentionally not part of this public specification:

- cost formulas
- duration formulas
- productivity models
- inflation models
- geotechnical influence logic
- procurement model effects
- risk probability and impact scoring
- deterministic mapping between L2 tokens and cost/time units
- BIM → quantity inference
- AI-token weighting algorithms

These remain internal BeeAi IP.

---

## 6. Extension Points (Public View)

- Sector-specific CTR shells
- International procurement-model variants
- Climate-aware timing structures
- Multi-scenario estimation models
- AI-assisted quality checks between CTR and feasibility layers

These reflect capability direction, not implementation.

---

## 7. Summary

The L6 Cost–Time–Risk Engine Layer provides a public structural view of BeeAi’s deterministic estimation model without disclosing proprietary logic.
It defines how information is organized while intentionally omitting calculations, formulas, weights, and mapping rules.
