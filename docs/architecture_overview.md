# Architecture Overview (Prototype)

## Goal
Provide a minimal but extensible **Digital Twin resilience prototype** that:
1. represents disruption states (S0–S3),
2. maps disruptions to indicator degradation,
3. applies tier-based activation policies,
4. visualizes scenario progression (demo video / web view),
5. supports reproducible simulation experiments.

## Core concepts
- **State model:** S0 (normal) → S1 (regional blackout) → S2 (physical attack) → S3 (adaptive recovery).
- **Indicators (KPIs):** Energy, Connectivity, Academic Continuity, Critical Services (extend as needed).
- **Tier activation:** Tier 1 (critical), Tier 2 (essential), Tier 3 (limited).
- **Policy:** decides which services remain powered/connected under constrained resources.

## Non-goals (for this prototype)
- Full physical power-grid modeling.
- Detailed cyber-physical causality and fault propagation.
- Real-time embedded execution constraints.
