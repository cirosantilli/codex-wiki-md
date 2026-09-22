# Zimm-Bragg model

↑ **Parent:** [Helix-coil transition model](helix-coil-transition-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zimm–Bragg_model)

A homogeneous Zimm-Bragg chain assigns propagation weight $s>0$ to each helical unit and initiation factor $\sigma>0$ to each helical run. With states ordered as coil and helix, one possible [transfer matrix for a classical spin chain](transfer-matrix-for-a-classical-spin-chain.md) is

$$
W=\begin{pmatrix}1&\sigma s\\1&s\end{pmatrix}.
$$

Its largest [eigenvalue](eigenvalue.md) is $\lambda_+=(1+s+\sqrt{(s-1)^2+4s\sigma})/2$. In the long-chain limit the [partition function](canonical-partition-function.md) grows as $\lambda_+^N$, so logarithmic differentiation gives the helical fraction $f_h=s\,\partial\ln\lambda_+/\partial s$, equal to the displayed expression. If $Q=(s-1)^2+4s\sigma$, then

$$
\frac{df_h}{ds}=\frac{\sigma(s+1)}{Q^{3/2}}>0,\qquad f_h(1)=\frac12,\qquad f_h'(1)=\frac1{4\sqrt\sigma}.
$$

For $\sigma=1$, $f_h=s/(1+s)$ and units are noncooperative. A small initiation factor suppresses boundaries and sharpens the crossover around $s=1$, with width of order $\sqrt\sigma$. For every fixed $\sigma>0$ the long-chain expression is smooth; a discontinuous step appears only in the singular $\sigma\downarrow0$ limit. [Theory of the Phase Transition between Helix and Random Coil in Polypeptide Chains, Journal of Chemical Physics 31 (1959), 526–535: propagation and initiation parameters and characteristic-matrix solution](https://doi.org/10.1063/1.1730390)

## ↑ Ancestors (6)

1. [Helix-coil transition model](helix-coil-transition-model.md)
2. [Biopolymer mechanics](biopolymer-mechanics.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Helix-coil transition model](helix-coil-transition-model.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018/section-b/b4/solution.md)
