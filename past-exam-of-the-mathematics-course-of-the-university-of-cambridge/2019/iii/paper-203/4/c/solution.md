<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $J_t=\psi_t'(U_t)$, $q_t=\psi_t''(U_t)/\psi_t'(U_t)$, and $r_t=(\partial_z^3\psi_t)(U_t)/\psi_t'(U_t)$. Since $dU_t=\sqrt{8/3}\,dB_t$, the supplied identity and [Itô formula](../../../../../../ito-s-lemma.md) give

$$
d\log J_t
=q_t\,dU_t
+\left[-\frac56q_t^2
+\left(-\frac43+\frac12\frac83\right)r_t\right]dt
=q_t\,dU_t-\frac56q_t^2dt.
$$

For $M_t=J_t^\alpha$, its drift coefficient is

$$
-\frac{5\alpha}{6}+\frac12\alpha^2\frac83
=\frac{\alpha(8\alpha-5)}6.
$$

Thus the nonzero choice is

$$
\boxed{\alpha=\frac58,}
$$

and $M_{t\wedge\tau}$ is a continuous local martingale. The boundary Schwarz lemma for mapping-out maps gives $0\leq J_{t\wedge\tau}\leq1$, so $0\leq M_{t\wedge\tau}\leq1$. A bounded local martingale is a true martingale. This is the [SLE eight-thirds restriction martingale](../../../../../../sle-eight-thirds-restriction-martingale.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
