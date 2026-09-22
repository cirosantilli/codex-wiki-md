<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $d=|x-y|\geq1$ and take $m=d-1$, so the [local projector cone in a frustration-free chain](../../../../../../../local-projector-cone-in-a-frustration-free-chain.md) for $A_{x(m)}$ does not contain $y$. It follows that $[A_{x(m)},B_y]=0$. The exact bra identity from (ii) and this commutation give

$$
\langle A_xB_y\rangle
=\langle A_{x(m)}B_y\rangle
=\langle B_yA_{x(m)}\rangle.
$$

Since $P_0A_x|\psi_0\rangle=\langle A_x\rangle|\psi_0\rangle$, subtracting the product of expectations yields

$$
\begin{aligned}
|\langle A_xB_y\rangle-\langle A_x\rangle\langle B_y\rangle|
&=\left|\langle\psi_0|B_y(A_{x(m)}-P_0A_x)|\psi_0\rangle\right|\\
&\leq q^{-2}\|A_x\|\|B_y\|q^{d-1}.
\end{aligned}
$$

Thus the [exponential clustering from layered projectors](../../../../../../../exponential-clustering-from-layered-projectors.md) bound is

$$
\boxed{|\langle A_xB_y\rangle-\langle A_x\rangle\langle B_y\rangle|
\leq q^{-3}\|A_x\|\|B_y\|e^{-\alpha d},
\qquad
\alpha=\frac13\ln\left(1+\frac{\Delta}{2}\right).}
$$

The [connected correlation function](../../../../../../../connected-correlation-function.md) therefore has correlation length at most $1/\alpha$ in lattice-spacing units. In particular $\alpha=\Delta/6+O(\Delta^2)$ for a small [spectral gap](../../../../../../../spectral-gap.md). The same-site case is covered by the elementary bound $2\|A_x\|\|B_y\|$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 67](../../../../paper-67-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
