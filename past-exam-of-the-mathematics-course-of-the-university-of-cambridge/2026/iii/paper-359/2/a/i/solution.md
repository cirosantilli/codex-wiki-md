<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the $L^2$ inner product of the first Galerkin equation with $\omega_m$. The [orthogonal projection](../../../../../../../orthogonal-projection.md) may be removed against $\omega_m\in\widetilde H_m$, and [skew-symmetry of incompressible transport](../../../../../../../skew-symmetry-of-incompressible-transport.md) cancels the nonlinear term. Hence

$$
\nu\|\nabla\omega_m\|_2^2+\gamma\|\omega_m\|_2^2
=(g,\omega_m).
$$

The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) and [Young inequality](../../../../../../../young-s-inequality-for-products.md) give

$$
\nu\|\nabla\omega_m\|_2^2+\frac{\gamma}{2}\|\omega_m\|_2^2
\leq\frac1{2\gamma}\|g\|_2^2.
$$

Thus both quantities requested in the first estimate are bounded by, for example,

$$
\boxed{R_1^2=\frac{\|g\|_2^2}{\gamma}}.
$$

Next take the inner product with $-\Delta\omega_m$. Periodicity and incompressibility give

$$
\begin{aligned}
\left|((u_m\mathbin\cdot\nabla)\omega_m,-\Delta\omega_m)\right|
&=\left|\int_\Omega\partial_j(u_m)_i\,\partial_i\omega_m\,\partial_j\omega_m\,dx\right|\\
&\leq \|\nabla u_m\|_2\|\nabla\omega_m\|_4^2.
\end{aligned}
$$

The given curl identity and the two-dimensional [Gagliardo-Nirenberg inequality](../../../../../../../gagliardo-nirenberg-interpolation-inequality.md) imply

$$
\|\nabla u_m\|_2\leq C\|\omega_m\|_2,
\qquad
\|\nabla\omega_m\|_4^2
\leq C\|\nabla\omega_m\|_2\|\Delta\omega_m\|_2.
$$

Applying Young's inequality to this term and to $(g,-\Delta\omega_m)$ yields

$$
\frac{\nu}{2}\|\Delta\omega_m\|_2^2
+\gamma\|\nabla\omega_m\|_2^2
\leq\frac{C}{\nu}
\left(\|g\|_2^2+\|\omega_m\|_2^2\|\nabla\omega_m\|_2^2\right).
$$

The first estimate bounds the right-hand side independently of $m$. Therefore one may choose a constant $R_2=R_2(\|g\|_2,\gamma,\nu,\mu_1)$ such that

$$
\boxed{\nu\|\Delta\omega_m\|_2^2\leq R_2^2,
\qquad
\gamma\|\nabla\omega_m\|_2^2\leq R_2^2}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
