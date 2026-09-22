<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $C=i/4$. Expanding

$$
S^{\lambda\mu\nu}=\frac12\bar\psi[\gamma^\lambda,\gamma^\mu]\gamma^\nu\psi
$$

with the [Clifford algebra](../../../../../../clifford-algebra.md), applying the product rule and then using the [Dirac equation](../../../../../../dirac-equation.md) and its adjoint gives

$$
\widehat T^{\mu\nu}
=T^{\mu\nu}+\frac i4\left[
\partial_\lambda S^{\lambda\mu\nu}
-\partial^\nu(\bar\psi\gamma^\mu\psi)
\right].
$$

This is the [Belinfante-Rosenfeld stress-energy tensor](../../../../../../belinfante-rosenfeld-stress-energy-tensor.md) written as an improvement of the canonical tensor.

The translation charges are

$$
P^\nu=\int d^3x\,T^{0\nu},
\qquad
\widehat P^\nu=\int d^3x\,\widehat T^{0\nu}.
$$

For spatial $\nu$, their difference is the integral of $\partial_iS^{i0\nu}-\partial^\nu(\bar\psi\gamma^0\psi)$. For $\nu=0$, use conservation of the [Dirac current](../../../../../../dirac-current.md) to replace $\partial^0(\bar\psi\gamma^0\psi)$ by a spatial divergence; also $S^{00\nu}=0$. Hence $\widehat P^\nu-P^\nu$ is always a spatial boundary integral. Under the usual decay boundary condition it vanishes, so both currents generate the same four-momentum.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
