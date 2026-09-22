<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a shortest path $x=x_0,\ldots,x_m=y$. Glue the prescribed one-step edge couplings successively. The [triangle inequality](../../../../../../triangle-inequality.md) for the Wasserstein transportation metric gives

$$
\rho_K(P(x,\cdot),P(y,\cdot))
\leq\sum_{j=1}^me^{-\alpha}\rho(x_{j-1},x_j)
=e^{-\alpha}\rho(x,y).
$$

Now couple initial states $(U,V)$ optimally for $\mu,\nu$ and conditionally use these one-step couplings. Taking expectations and then the infimum gives

$$
\rho_K(\mu P,\nu P)\leq e^{-\alpha}\rho_K(\mu,\nu).
$$

Iteration with $\nu=\pi$ yields $\rho_K(P^t(x,\cdot),\pi)\leq e^{-\alpha t}\operatorname{diam}(V)$. Since this metric dominates total variation, it is at most $\varepsilon$ once

$$
\boxed{t\geq\frac1\alpha\left(\log\operatorname{diam}(V)+\log(1/\varepsilon)\right).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
