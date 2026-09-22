<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $W=Z-\mathbb EZ$ and $\psi(\lambda)=\log\mathbb E_Pe^{\lambda W}$. For any $Q\ll P$ and real $\lambda$, define the exponential tilt

$$
\frac{dP_\lambda}{dP}=e^{\lambda W-\psi(\lambda)}.
$$

Positivity of relative entropy gives

$$
D(Q\Vert P)=D(Q\Vert P_\lambda)
+\lambda\mathbb E_QW-\psi(\lambda)
\geq\lambda\mathbb E_QW-\psi(\lambda).
$$

Thus every $Q$ with $\mathbb E_QW\geq t$ has $D(Q\Vert P)\geq\sup_{\lambda\geq0}\{\lambda t-\psi(\lambda)\}=\psi^*(t)$.

For $0<t<b$, continuity of $\psi'$ supplies $\lambda_t>0$ with $\psi'(\lambda_t)=t$. Under $P_{\lambda_t}$, $\mathbb EW=t$, and direct substitution gives

$$
D(P_{\lambda_t}\Vert P)
=\lambda_t t-\psi(\lambda_t)=\psi^*(t).
$$

This tilt attains the constrained infimum and proves the identity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
