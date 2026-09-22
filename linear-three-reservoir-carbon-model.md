# Linear three-reservoir carbon model

↑ **Parent:** [Atmospheric chemistry](atmospheric-chemistry.md)

A capacity-weighted exchange model for atmospheric, fast surface and deep [ocean](ocean.md) [carbon dioxide](carbon-dioxide.md) anomalies. Positive diagonal capacities form $D$, while $L$ is the weighted path-graph [Laplacian matrix](laplacian-matrix.md) with exchange conductances $r,s$. Then $\mathbf C^TL\mathbf C=r(C_a-C_b)^2+s(C_b-C_d)^2\geq0$. The homogeneous generator $-D^{-1}L$ is similar to a symmetric negative-semidefinite [matrix](matrix.md), with two decaying [normal modes](normal-mode.md) and one zero [normal mode](normal-mode.md) for equal concentrations. Summing all budgets proves that the capacity-weighted total is conserved after emissions stop. The long-time concentration from total input $M$ is $M/(R_a+R_b+R_d)$, rather than zero.

## ↑ Ancestors (3)

1. [Atmospheric chemistry](atmospheric-chemistry.md)
2. [Chemistry](chemistry-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford/2022/5/b/solution.md)
