# Pending infections at quarantine in a delayed epidemic model

↑ **Parent:** [Quarantine threshold in the SIR model](quarantine-threshold-in-the-sir-model.md)

When exposed animals remain in a not-yet-infective [compartment](compartmental-models-epidemiology.md) for a fixed [incubation period](incubation-period.md) $\tau$, stopping all new exposure does not cancel the pending case transfers. At isolation time $T$, their number is $E(T)=\int_{T-\tau}^{T}rI(s)S(s)\,ds=\tau rI(T)S(T)+O(\tau^2)$ for smooth profiles. Eventual [cases](infectious-disease.md) therefore include this pipeline in addition to case transfers already completed by $T$. The interpretation depends on the [compartment](compartmental-models-epidemiology.md) definition: a strictly unexposed [susceptible](susceptible-individual.md) [compartment](compartmental-models-epidemiology.md) would instead lose these animals at exposure.

## ↑ Ancestors (7)

1. [Quarantine threshold in the SIR model](quarantine-threshold-in-the-sir-model.md)
2. [Quarantine](quarantine.md)
3. [Mathematical epidemiology](mathematical-epidemiology.md)
4. [Mathematical biology](mathematical-biology-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
