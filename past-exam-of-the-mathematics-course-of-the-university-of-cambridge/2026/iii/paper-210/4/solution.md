<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [pushforward measure](../../../../../pushforward-measure.md) of $\mu$ under $g$ is $g_*\mu$, defined for $B\in\mathcal B$ by

$$
(g_*\mu)(B)=\mu(g^{-1}(B)).
$$

The [Lebesgue decomposition theorem](../../../../../lebesgue-decomposition-theorem.md) says that if $\nu$ and $\mu$ are sigma-finite measures on the same measurable space, then uniquely

$$
\nu=\nu_{\mathrm{ac}}+\nu_{\mathrm{s}},
\qquad \nu_{\mathrm{ac}}\ll\mu,
\qquad \nu_{\mathrm{s}}\perp\mu.
$$

Let $f:[0,\infty)\to\mathbb R\cup{+\infty}$ be [convex](../../../../../convex-function.md) with $f(1)=0$. If $\lambda$ dominates the [probability distributions](../../../../../probability-distribution.md) $P,Q$, with densities $p,q$, their [f-divergence](../../../../../f-divergence.md) is

$$
D_f(P\Vert Q)=\int q,f(p/q)\,d\lambda,
$$

using the lower-semicontinuous perspective convention where $q=0$. This definition is independent of the dominating measure.

The [data processing inequality for f-divergences](../../../../../data-processing-inequality-for-f-divergences.md) states

$$
D_f(g_*P\Vert g_*Q)\leq D_f(P\Vert Q).
$$

To prove it, take $\lambda=P+Q$ and let $\mathcal G=g^{-1}(\mathcal B)$. If $p=dP/d\lambda$ and $q=dQ/d\lambda$, then the pullbacks of the densities of $g_*P$ and $g_*Q$ with respect to $g_*\lambda$ are respectively $\mathbb E_\lambda[p\mid\mathcal G]$ and $\mathbb E_\lambda[q\mid\mathcal G]$. The perspective $F(a,b)=bf(a/b)$ of a convex function is jointly convex. Conditional [Jensen inequality](../../../../../jensen-s-inequality.md) therefore gives

$$
F(\mathbb E[p\mid\mathcal G],\mathbb E[q\mid\mathcal G])
\leq\mathbb E[F(p,q)\mid\mathcal G].
$$

Integration proves the claim.

The [Squared Hellinger distance](../../../../../squared-hellinger-distance.md) is

$$
H^2(P,Q)=\int\left(\sqrt{dP/d\lambda}-\sqrt{dQ/d\lambda}\right)^2d\lambda.
$$

If $P,Q$ have densities $p,q$ with respect to a sigma-finite measure $\mu$, this becomes

$$
H^2(P,Q)=\int(\sqrt p-\sqrt q)^2d\mu
=2-2\int\sqrt{pq}\,d\mu.
$$

Fix any probability distribution $Q$ and set $p_j=P_j(A_j)$, $q_j=Q(A_j)$, and $t_j=H^2(P_j,Q)$. Applying the data processing inequality to the [indicator function](../../../../../indicator-function.md) of $A_j$ gives the Bernoulli Hellinger bound

$$
t_j\geq2-2\left(\sqrt{p_jq_j}+\sqrt{(1-p_j)(1-q_j)}\right).
$$

The hinted inequality implies

$$
(p_j-q_j)^2\leq t_j\left(1-\frac{t_j}{4}\right).
$$

The function $t\mapsto\sqrt{t(1-t/4)}$ is concave on $[0,2]$. Since the $A_j$ form a [set partition](../../../../../set-partition.md), $\sum_jq_j=1$, and [Jensen inequality](../../../../../jensen-s-inequality.md) gives

$$
\begin{aligned}
\frac1M\sum_{j=1}^MP_j(A_j)
&\leq\frac1M+\frac1M\sum_{j=1}^M
\sqrt{t_j(1-t_j/4)}\\
&\leq\frac1M+
\sqrt{\frac1M\sum_{j=1}^Mt_j}
\sqrt{1-\frac1{4M}\sum_{j=1}^Mt_j}.
\end{aligned}
$$

Taking the infimum over $Q$ proves the stated inequality.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
