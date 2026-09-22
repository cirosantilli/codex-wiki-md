<h1 id="2/2/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Suppose that $T=\infty$. Since $s_c<1$ and $d\geq3$,

$$
p<1+\frac4{d-2}\leq5.
$$

The [Radial Sobolev inequality](../../../../../../../radial-sobolev-inequality.md) and [Mass conservation for the nonlinear Schrödinger equation](../../../../../../../mass-conservation-for-the-nonlinear-schrodinger-equation.md) give

$$
\int_{|x|\geq2R}|u|^{p+1}
\leq C(u_0)R^{-(d-1)(p-1)/2}
\|\nabla u\|_2^{(p-1)/2}.
$$

Because $(p-1)/2<2$, [Young inequality](../../../../../../../young-s-inequality-for-products.md) and a sufficiently large fixed $R$ absorb this term into the left side of the estimate from part 5. The annular term is at most $C(u_0)R^{-2}$. Using the uniform lower bound $\|\nabla u(t)\|_2\geq c(u_0)$ from part 2 and enlarging $R$ once more yields

$$
V_{\psi_R}'(t)\leq-\delta(u_0)<0.
$$

Since $I_{\psi_R}'=2V_{\psi_R}$, two integrations give

$$
I_{\psi_R}(t)
\leq I_{\psi_R}(0)+2V_{\psi_R}(0)t-\delta t^2.
$$

The right-hand side is negative for large $t$, contradicting $I_{\psi_R}(t)=\int\psi_R|u|^2\geq0$. Hence the maximal forward lifespan is finite: $T<\infty$.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
