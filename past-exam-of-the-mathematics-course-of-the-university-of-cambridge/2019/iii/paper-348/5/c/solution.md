<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $L=W_p(\mu,\nu)$. The assumed equality of the [Monge optimal transport problem](../../../../../../monge-optimal-transport-problem.md) and [Kantorovich optimal transport problem](../../../../../../kantorovich-optimal-transport-problem.md) values gives

$$
\int|T^\dagger(x)-x|^p\,d\mu(x)=L^p.
$$

Each interpolated [pushforward measure](../../../../../../pushforward-measure.md) $\mu_t=(P_t)_\#\mu$ has a finite $p$th [absolute moment](../../../../../../absolute-moment.md), since $|P_t(x)|^p\leq2^{p-1}(|x|^p+|T^\dagger(x)|^p)$ and $(T^\dagger)_\#\mu=\nu$.

For any $s,t\in[0,1]$, the common-source [transport plan](../../../../../../transport-plan.md)

$$
\pi_{s,t}=(P_s,P_t)_\#\mu\in\Pi(\mu_s,\mu_t)
$$

provides the upper bound

$$
W_p(\mu_s,\mu_t)^p\leq\int|P_t(x)-P_s(x)|^p\,d\mu
=|t-s|^p L^p.
$$

For the reverse bound assume $0\leq s\leq t\leq1$. Since $\mu_0=\mu$ and $\mu_1=\nu$, the [triangle inequality](../../../../../../triangle-inequality.md) for the [p-Wasserstein distance](../../../../../../p-wasserstein-distance.md) and the upper bounds already established give

$$
\begin{aligned}
L&\leq W_p(\mu_0,\mu_s)+W_p(\mu_s,\mu_t)+W_p(\mu_t,\mu_1)\\
&\leq sL+W_p(\mu_s,\mu_t)+(1-t)L.
\end{aligned}
$$

Hence $W_p(\mu_s,\mu_t)\geq(t-s)L$. Combining the bounds and using symmetry proves

$$
\boxed{W_p(\mu_t,\mu_s)=|t-s|W_p(\mu,\nu).}
$$

This is the constant speed property of [displacement interpolation](../../../../../../displacement-interpolation.md). The given invertibility of $P_s$ also lets one realize the competitor as the map $P_t\circ P_s^{-1}$, assuming its inverse is measurable, but the [transport plan](../../../../../../transport-plan.md) argument proves the result without invertibility.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
