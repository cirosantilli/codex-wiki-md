<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

On the finite-dimensional space $H_m$, the Galerkin equation is an autonomous system of ordinary differential equations whose right-hand side is a quadratic polynomial in the coefficients of $u_m$. It is locally Lipschitz, so the [Picard-Lindelöf theorem](../../../../../../../picard-lindelof-theorem.md) gives a unique maximal local solution.

Taking the $H$ inner product with $u_m$ gives

$$
\frac12\frac d{dt}|u_m|^2+\nu\|u_m\|^2
+\langle B(P_Nu_m,u_m),u_m\rangle=0.
$$

The advecting field $P_Nu_m$ is divergence free. Periodicity and the [skew-symmetry of incompressible transport](../../../../../../../skew-symmetry-of-incompressible-transport.md) therefore make the nonlinear term zero. Hence

$$
|u_m(t)|\leq|P_mu_0|\leq|u_0|.
$$

A finite-dimensional solution can cease to exist only if its norm diverges. This uniform bound prevents such blow-up, so the solution extends uniquely through every interval $[0,T]$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
