<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove the extension from spatial test functions to **[time-dependent test functions for a diffusion martingale problem](../../../../../../time-dependent-test-functions-for-a-diffusion-martingale-problem.md)** directly, without assuming a driving [Brownian motion](../../../../../../brownian-motion-split.md). Fix $0\leq s<t$ and a deterministic partition $s=t_0<\cdots<t_n=t$. For each $j$, $g_j(x)=f(t_j,x)$ lies in $C_b^2$. The defining [martingale problem](../../../../../../martingale-problem.md) gives

$$
\mathbb E\left[\mathbf1_A\sum_{j=0}^{n-1}\left(f(t_j,X_{t_{j+1}})-f(t_j,X_{t_j})-\int_{t_j}^{t_{j+1}}Lf(t_j,X_u)du\right)\right]=0\qquad(A\in\mathcal F_s).
$$

Call the sum $S_n$. Telescoping separates the spatial and temporal changes:

$$
S_n=f(t,X_t)-f(s,X_s)-\sum_j\int_{t_j}^{t_{j+1}}\partial_u f(u,X_{t_{j+1}})du-\sum_j\int_{t_j}^{t_{j+1}}Lf(t_j,X_u)du.
$$

The sample path $X$ is uniformly continuous on $[s,t]$ and has compact range. Joint continuity of $\partial_t f$, the spatial first derivatives, and the spatial second derivatives therefore gives, as the mesh tends to zero,

$$
S_n\longrightarrow f(t,X_t)-f(s,X_s)-\int_s^t(\partial_u+L)f(u,X_u)du=M_t^f-M_s^f
$$

almost surely. For bounded $a,b$ and bounded derivatives of $f$, both integrals are uniformly bounded on this finite horizon, as are the two endpoint terms. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) permits passage to the limit in the expectation against $\mathbf1_A$. Thus $M_t^f$ is integrable and $\mathbb E[\mathbf1_A(M_t^f-M_s^f)]=0$ for every $A\in\mathcal F_s$, proving

$$
\boxed{\mathbb E[M_t^f\mid\mathcal F_s]=M_s^f.}
$$

Adaptation and continuity follow from the formula, so **$M^f$ is a continuous [martingale](../../../../../../martingale-split.md)**. Under the more general integrability condition in part (a), the same proof uses an integrable bound proportional to $1+\int_s^t(\sum_i|b_i(X_u)|+\sum_i a_{ii}(X_u))du$; positive semidefiniteness bounds every off-diagonal entry by the diagonal ones. With only local assumptions this reasoning proves a [local martingale](../../../../../../local-martingale.md), and an integrability hypothesis is needed to upgrade that conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
