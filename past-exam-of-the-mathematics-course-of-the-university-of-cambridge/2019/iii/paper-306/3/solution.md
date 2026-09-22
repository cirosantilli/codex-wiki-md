<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [BRST operator](../../../../../brst-operator.md) $Q_B$ is Grassmann odd and represents the gauge symmetry on the gauge-fixed state space. Requiring two successive BRST transformations to vanish means

$$
Q_B^2=\frac12\{Q_B,Q_B\}=0.
$$

This nilpotence makes physical states a [BRST cohomology](../../../../../brst-cohomology.md). If $[Q_B,S_0]=0$ and $\Psi$ is the [gauge-fixing fermion](../../../../../gauge-fixing-fermion.md), the graded Jacobi identity gives

$$
[Q_B,S]=[Q_B,S_0]+[Q_B,\{Q_B,\Psi\}]
=\frac12[\{Q_B,Q_B\},\Psi]=0,
$$

so $S=S_0+\{Q_B,\Psi\}$ is BRST invariant.

A holomorphic field of [conformal weight](../../../../../conformal-weight.md) $h$ has the Laurent expansion

$$
\phi(z)=\sum_{n\in\mathbb Z}\phi_nz^{-n-h}.
$$

Under the [state–operator correspondence](../../../../../state-operator-correspondence.md), $\phi(z)|0\rangle$ must be regular at the origin. Terms with $n>-h$ have negative powers, so

$$
\boxed{\phi_n|0\rangle=0\quad(n>-h)}.
$$

For the anticommuting [bc system](../../../../../bc-system.md),

$$
b(z)=\sum_nb_nz^{-n-2},\qquad c(z)=\sum_nc_nz^{-n+1},
\qquad\{b_m,c_n\}=\delta_{m+n,0}.
$$

Separating creation and annihilation modes and summing the geometric series for $|z|>|w|$ gives the [bc ghost operator-product expansion](../../../../../bc-ghost-operator-product-expansion.md)

$$
\boxed{b(z)c(w)\sim\frac1{z-w}}.
$$

The [BRST current](../../../../../brst-current.md) built from the matter and ghost stress tensors has an operator-product expansion with $c$ whose residue gives

$$
\boxed{\{Q_B,c(z)\}=c(z)\partial c(z)}.
$$

For a matter [Virasoro primary operator](../../../../../primary-field.md) $\Phi(z,\bar z)$ of weights $(1,1)$, the two standard [string vertex operators](../../../../../string-vertex-operator.md) are

$$
\boxed{U(z,\bar z)=c(z)\bar c(\bar z)\Phi(z,\bar z)},
\qquad
\boxed{V=\int_\Sigma d^2z\,\Phi(z,\bar z)}.
$$

The first is the local, unintegrated vertex. Using $Q_Bc=c\partial c$, $Q_B\bar c=\bar c\bar\partial\bar c$, and the weight-$(1,1)$ transformation of $\Phi$, the terms cancel pairwise and $Q_BU=0$. For the integrated vertex,

$$
\{Q_B,\Phi\}=\partial(c\Phi)+\bar\partial(\bar c\Phi),
$$

so $\{Q_B,V\}=0$ on a closed worldsheet because the variation is a total derivative. Both vertices therefore represent the same [BRST cohomology](../../../../../brst-cohomology.md) class.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
