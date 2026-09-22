# Persistence correction to a gene-circuit pulse threshold

↑ **Parent:** [Logic approximation for gene regulation](logic-approximation-for-gene-regulation.md)

Suppose an input is produced for time $T$, then decays, and activates two identical mutually activating OR-gated outputs. Write $S=\beta/\alpha$ and $h=K/S\in(0,1)$. The input remains above threshold until $\alpha^{-1}\ln[(e^{\alpha T}-1)/h]$. Each output reaches threshold at $-2\ln(1-h)/\alpha$ if input remains available. Equating these times gives the limiting pulse duration $T_{\min}=\alpha^{-1}\ln[1+h/(1-h)^2]$. Exact equality depends on the ideal gate's boundary convention; a robust latch requires a longer pulse. Treating cessation of production as immediate removal incorrectly discards the input's residual lifetime.

## ↑ Ancestors (6)

1. [Logic approximation for gene regulation](logic-approximation-for-gene-regulation.md)
2. [Gene regulatory network](gene-regulatory-network.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-biological-physics-course-of-the-university-of-oxford/2019/3/b/solution.md)
