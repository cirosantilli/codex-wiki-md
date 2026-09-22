<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [Levi-Civita connection](../../../../../../levi-civita-connection.md), the background metric is constant and replacing $g^{\alpha\rho}$ by its $O(\epsilon)$ correction would multiply a derivative of $h$ and produce an $O(\epsilon^2)$ term. Hence the [linearized Levi-Civita connection](../../../../../../linearized-levi-civita-connection.md) is

$$
\boxed{
\Gamma^\alpha{}_{\beta\gamma}
=\frac12\eta^{\alpha\rho}
\left(
\partial_\beta h_{\gamma\rho}
+\partial_\gamma h_{\beta\rho}
-\partial_\rho h_{\beta\gamma}
\right)}.
$$

The products of two connection coefficients in the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) are also quadratic and may be discarded. Lowering its first index with $\eta_{\mu\nu}$ gives

$$
\boxed{
R_{\mu\rho\alpha\beta}^{(1)}
=\frac12\left(
\partial_\alpha\partial_\rho h_{\mu\beta}
-\partial_\alpha\partial_\mu h_{\rho\beta}
-\partial_\beta\partial_\rho h_{\mu\alpha}
+\partial_\beta\partial_\mu h_{\rho\alpha}
\right)}.
$$

Because the coordinate change is $\widetilde x^\alpha=x^\alpha-\xi^\alpha$, the perturbation changes at linear order by

$$
\widetilde h_{\mu\nu}
=h_{\mu\nu}+\partial_\mu\xi_\nu+\partial_\nu\xi_\mu.
$$

Substitution into $R_{\mu\rho\alpha\beta}^{(1)}$ produces terms containing three partial derivatives of $\xi$. Since partial derivatives commute, every term cancels another with the opposite sign. Therefore

$$
\boxed{\widetilde R_{\mu\rho\alpha\beta}^{(1)}
=R_{\mu\rho\alpha\beta}^{(1)}}.
$$

This is the [gauge invariance of the linearized Riemann tensor](../../../../../../gauge-invariance-of-the-linearized-riemann-tensor.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 357](../../../paper-357-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
