# Infection-triggered vaccination model

↑ **Parent:** [SIR model](sir-model.md)

A fatal-infection model with [vaccination](vaccination.md) proportional to infective-susceptible encounters adds $v_t=\eta qs$ and $m_t=q$. The total count including deaths is conserved. Integrating $dq/ds$ and $dv/ds$ gives $q=q_0+[s_0-s+\log(s/s_0)]/(1+\eta)$ and $v=\eta(s_0-s)/(1+\eta)$. The selected final root has $0<s_\infty<\min(s_0,1)$, and deaths are $q_0+(s_0-s_\infty)/(1+\eta)$. The model is a specified deterministic reaction scheme, not a general [vaccination](vaccination.md) policy rule.

## ↑ Ancestors (6)

1. [SIR model](sir-model.md)
2. [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
