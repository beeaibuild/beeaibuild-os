# BeeAi OS Kernel – L2 Token Layer Specification
### Neutral Structured Token Model → Cross-Sector Reasoning Backbone

The L2 Layer defines the **structured, neutral data units** (“tokens”) that allow BeeAi to reason consistently about infrastructure projects across sectors.  
While L1 captures *functional intent*, L2 provides the **standardized building blocks** necessary for early-stage analysis, comparison, and downstream mapping.

L2 = **Structured Token Model.**  
It transforms L1 intent into reusable, comparable, domain-agnostic elements without exposing any proprietary logic.

---

## ### 1. Purpose of the L2 Token Layer

The L2 Token Layer provides a unified structure that BeeAi OS uses to represent:

- project context  
- functional components  
- influencing complexity factors  
- lifecycle phases  

It enables early-stage estimation and cross-sector reasoning without requiring domain-specific data or sector ontology access.

This public specification intentionally omits private mapping logic, weights, and calculation methods.

---

## ### 2. High-Level Concept

L2 tokens are **abstracted descriptors** of a project’s environment and functional composition.  
They serve as the common language between:

- L1 functional intent  
- L3 sector ontologies  
- downstream engines (permitting, cost–time–risk, feasibility, compliance)

The token layer ensures that any project can be interpreted using a **shared vocabulary**.

---

## ### 3. Token Categories (Public Simplified Set)

### **3.1 Project-Context Tokens**
Describe where the project exists.

Examples:
- `zone_type` (urban / suburban / rural)
- `regulatory_class` (public works / private development)
- `climate_band` (A–F bands)
- `site_access` (easy / moderate / constrained)

> Deep geotechnical, hydrological, and utility-mapping attributes remain private and are *not* part of this public spec.

---

### **3.2 Functional Tokens**
Represent abstract units of infrastructure.

Examples:
- `transport_corridor`
- `utility_distribution_segment`
- `public_facility_core_unit`

These link to L3 sector ontologies without revealing their internal structure.

---

### **3.3 Complexity Tokens**
Capture contextual factors that influence uncertainty and risk.

Examples:
- `right_of_way_constraint`
- `environmental_sensitivity`
- `stakeholder_density`

No proprietary weighting or scoring logic is included.

---

### **3.4 Phase Tokens**
Neutral representation of lifecycle phases:

- `phase_planning`
- `phase_permitting`
- `phase_design_basic`
- `phase_design_detailed`
- `phase_construction`
- `phase_handover`

These ensure uniform temporal reasoning across sectors.

---

## ### 4. Token Structure (Public Minimal Format)

```json
{
  "token_id": "string",
  "category": "context | functional | complexity | phase",
  "attributes": {
    "name": "string",
    "descriptor": "string",
    "level": "L2"
  },
  "links": {
    "l1_ref": "functional_intent_id",
    "l3_ref": ["optional_domain_links"]
  }
}
```
This format captures the shape of the token architecture without exposing underlying logic, formulas, or mappings.

---

## ###5 Interaction With L1 and L3 Layers

L1 → L2

L1 provides what the project must achieve.
L2 converts this into structured, comparable elements.

L2 → L3

L2 tokens connect to sector ontologies (transport, utilities, buildings, government).
The mapping logic itself remains private.

---

## ### 6. Intended Extension Points (Public View)

- Additional sector mappings via L3
- Expanded context and complexity token sets
- Multinational regulatory classifications
- Integration with permitting knowledge bases
- Climate and terrain factor extensions

These highlight architectural direction without revealing the operational engine.

---

## ### 7. Explicitly Out of Scope (Private Components)

The following are intentionally not included in this public specification:

- cost logic
- time / duration logic
- risk scoring logic
- geotechnical transformation
- AI-token generation rules
- BIM → autodetails pipeline
- deterministic mapping and weighting models
- proprietary sector ontologies

These remain part of BeeAi’s private IP.

---

## ### 8. Summary

The L2 Token Layer defines the neutral reasoning vocabulary that enables BeeAi OS to analyze any infrastructure project at an early stage.
It forms the bridge between human intent (L1) and sector-specific domain models (L3), while protecting all proprietary logic and algorithms.
