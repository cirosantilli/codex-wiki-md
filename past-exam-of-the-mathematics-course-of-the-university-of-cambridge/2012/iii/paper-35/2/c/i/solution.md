<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Restrict $\mu$ first to loops surrounding $0$. This satisfies the pointed restriction property, so for one constant $C$,

$$
\boxed{\mu_D\big|_{E_0}=C\,\Gamma_*\rho.}
$$

A single rooted pushforward cannot equal the whole $\mu_D$: it only sees loops surrounding its root. The rest is recovered by moving that root.

For $z\in D$, choose a disc automorphism $\psi_z$ with $\psi_z(0)=z$. Conformal restriction yields

$$
\mu_D\big|_{E_z}=C\,(\psi_z\circ\Gamma)_*\rho,
$$

with the same constant. Let $(z_j)$ be a countable dense set in $D$. Every simple loop contained in $D$ surrounds one of these points. Make this cover disjoint by $P_j=E_{z_j}\setminus\bigcup_{i<j}E_{z_i}$. For a measurable event $A$ of loops in $D$,

$$
\boxed{\mu_D(A)=C\sum_j\rho\{B:\psi_{z_j}(\Gamma(B))\in A\cap P_j\}.}
$$

This explicitly relates the entire loop measure to the single-root measure without overcounting a loop once for every point in its interior. It also proves that knowledge of $\rho$, up to normalization, determines $\mu_D$. Nontriviality gives $C>0$: otherwise all countably many pointed patches would vanish. Using the usual unrooted [Brownian loop measure](../../../../../../../brownian-loop-measure.md), the same construction is commonly expressed as its outer-boundary pushforward, up to a constant.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
