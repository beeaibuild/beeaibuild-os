# Example: Data Center Infrastructure (Concept)

Demonstrates how BeeAiBUILD-OS structures an early-stage hyperscale server-farm request.

## Intent
Evaluate feasibility, constraints, and utility dependencies for a hyperscale data center development.

## SIM
type: data center (server farm)  
capacity: 12 MW IT load  
site area: ~6 ha  
cooling: hybrid (liquid + air)  
grid connection: required (132 kV)  

## Tokens Triggered
ENG.ELEC_LOAD_011  
ENG.COOLING_CAPACITY_007  
REG.ZONING_TECH_003  
PM.UTILITY_DEPENDENCY_014  
RISK.GRID_LEADTIME_002  

## Output (CTR Shell – structure only)
feasible: CONDITIONAL  
constraints: high-voltage grid availability, cooling-system siting  
risks: long utility-lead-time, transformer procurement, noise envelope  
timeline: 24–30 months (band estimate)  
cost envelope: C2–C4 (major uncertainty: grid upgrades)
