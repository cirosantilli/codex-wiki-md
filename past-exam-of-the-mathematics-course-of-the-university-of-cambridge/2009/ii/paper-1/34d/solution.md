<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

For a normalized trial function in the quadratic-form domain of the [Schrödinger operator](../../../../../schrodinger-operator.md), integration by parts gives $\langle E\rangle=\langle\psi,H\psi\rangle$. Expand in the complete orthonormal [energy eigenstates](../../../../../energy-eigenstate.md), $\psi=\sum_nc_n\psi_n$ with $\sum_nc_n^2=1$. Then

$$
\langle E\rangle=\sum_nE_nc_n^2\geq E_0\sum_nc_n^2=E_0.
$$

Minimizing over a trial family therefore gives the best upper bound within that family, the [quantum variational principle](../../../../../quantum-variational-principle.md).

For $V=|x|$, choose $\psi_\alpha=(\alpha/\pi)^{1/4}e^{-\alpha x^2/2}$ with $\alpha>0$. The Gaussian integrals give

$$
\int(\psi_\alpha')^2dx=\frac\alpha2,\qquad
\int|x|\psi_\alpha^2dx=\frac1{\sqrt{\pi\alpha}}.
$$

Thus $E(\alpha)=\alpha/2+(\pi\alpha)^{-1/2}$, whose derivative vanishes at $\alpha=\pi^{-1/3}$. It tends to infinity at both parameter endpoints and has positive second derivative, so this is its minimum. **$\boxed{E_0\leq\tfrac32\pi^{-1/3}\simeq1.0242}$** is the resulting estimate.

The potential is even; the unique nodeless ground state is even and the first excited state is odd, by the one-dimensional [Sturm oscillation theorem](../../../../../sturm-oscillation-theorem.md). To estimate $E_1$, minimize the same [Rayleigh quotient](../../../../../rayleigh-quotient.md) over odd trial functions, for example normalized $x e^{-\alpha x^2/2}$, or the compactly supported odd family $C_a x(1-|x|/a)$ for $|x|\leq a$ and zero otherwise. Oddness gives exact orthogonality to the true ground state, not merely to an approximate trial ground state. The [quantum variational principle](../../../../../quantum-variational-principle.md) restricted to the odd sector supplies an upper bound for $E_1$. No further integration is needed.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
