# BeeAi OS – Glossary
### Core Terms of the Kernel Architecture

This glossary defines the key concepts used throughout the BeeAi OS Kernel.  
All terms are architecture-level abstractions and contain no proprietary logic.

---

## 1. Intent Layer Terms

### **Functional Intent (L1)**
High-level description of *what the project must accomplish*.  
Machine-readable representation of human goals, constraints, and functional scope.

### **Intent Object**
The structured data unit that stores L1 intent elements.

---

## 2. Token Layer Terms

### **Token (L2)**
A neutral, structured element representing:
- context  
- functional components  
- complexity factors  
- lifecycle phases  

Tokens enable cross-sector reasoning without domain rules.

### **Token Category**
Classification of tokens by their purpose:
- context  
- functional  
- complexity  
- phase  

### **Token Mapping**
Non-public internal transformation linking tokens to domain models.  
Not included in the public spec.

---

## 3. Ontology Layer Terms

### **Sector Ontology (L3)**
Domain-specific structural model describing what infrastructure components *are* in each sector.

### **Ontology Node**
Atomic element of an ontology representing a domain component.

### **Ontology Link**
Reference from an ontology node to related L2 tokens.  
Mapping logic remains private.

---

## 4. Permitting Layer Terms

### **Permit Cluster (L4)**
A grouped regulatory requirement or approval step relevant to the project.

### **Regulatory Actor**
Authority or stakeholder responsible for reviewing or approving a cluster.

### **Dependency Chain**
Ordered sequence in which permit clusters must be addressed.

### **Approval Gate**
Key milestone where a project enters or exits a regulatory phase.

---

## 5. Feasibility Layer Terms

### **Feasibility Constraint (L5)**
A structural issue that may affect viability:
- physical  
- regulatory  
- functional  
- stakeholder  

### **Constraint Group**
Collection of constraints within the same category.

### **Alignment Check**
High-level indication of whether project representation across L1–L4 is coherent.

---

## 6. Cost–Time–Risk Layer Terms

### **CTR Shell (L6)**
A non-calculated, structural placeholder representing:
- cost group  
- duration phase  
- risk group  

### **Cost Group Shell**
Conceptual placeholder for cost components without formulas.

### **Phase Duration Shell**
Neutral representation of project duration blocks.

### **Risk Flag**
Qualitative indication of a potential risk area (no scoring).

---

## 7. Cross-Layer Terms

### **Reasoning Surface**
A structured layer providing deterministic, interpretable information to the next layer.

### **Neutral Model**
A representation free of jurisdiction-specific rules, formulas, or proprietary logic.

### **Deterministic Structure**
A model that guarantees consistent interpretation independent of input variations.

---

## 8. Out-of-Scope Terms

The following terms exist in BeeAi but are NOT part of the public specification:
- AI-token weighting  
- BIM-to-autodetail mapping  
- quantitative estimation models  
- procurement logic  
- geotechnical influence rules  
- country-specific permitting rules  

These are private and not documented here.

---

## 9. Summary

This glossary standardizes the vocabulary used across the BeeAi OS Kernel.  
It ensures clarity, consistency, and architectural integrity across layers.

---
