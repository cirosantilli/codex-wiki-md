<h1 id="3/3/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Choose a smooth radial cutoff $\theta_R$ that vanishes on $|x|\leq R$, equals one on $|x|\geq2R$, and satisfies $|\nabla\theta_R|\leq C/R$. The first [localized virial identity](../../../../../../../localized-virial-identity.md) and the estimate from part 2, applied to $w=u(t)$ and $\psi=\theta_R$, give

$$
\left|\frac d{dt}\int\theta_R|u(t)|^2\right|
\leq\frac{C(u_0)}R,
$$

because the mass and energy are conserved.

For fixed $R$, the strong profile convergence from part 5 and $\lambda_n\to0$ imply

$$
\int\theta_R(x)|u(t_n,x)|^2,dx
=\int\theta_R(\lambda_n y)|v_n(y)|^2,dy\longrightarrow0.
$$

Integrating the flux estimate from $t$ to $t_n$ and then letting $n\to\infty$ yields

$$
\int_{|x|\geq2R}|u(t,x)|^2,dx
\leq\frac{C(u_0)T}{R}
$$

uniformly for $0\leq t<T$. Taking $R$ sufficiently large proves the claim.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
