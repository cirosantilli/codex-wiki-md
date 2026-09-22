<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For an elementary [previsible](../../../../../../predictable-process.md) integrand, the integral is the increment sum $\sum_jH_j(X_{t\wedge t_{j+1}}-X_{t\wedge t_j})$. This expression uses only $H$ and $X$, so is identical under the two measures, irrespective of how the [local martingale](../../../../../../local-martingale.md) and finite-variation parts change.

We may use the [stochastic dominated convergence theorem](../../../../../../stochastic-dominated-convergence-theorem.md): if bounded [predictable](../../../../../../predictable-process.md) $H_n$ converge pointwise to $H$ under a common deterministic bound, their integrals against a [semimartingale](../../../../../../semimartingale.md) converge uniformly on compact intervals in probability. Also convergence in $\mathbb P$-probability implies convergence in $\mathbb Q$-probability when $\mathbb Q\ll\mathbb P$. To see the latter directly, let $D=d\mathbb Q/d\mathbb P$. For any event $E$,

$$
\mathbb Q(E)=\mathbb E_{\mathbb P}(D\mathbf1_E)\le K\mathbb P(E)+\mathbb E_{\mathbb P}(D\mathbf1_{\{D>K\}}),
$$

and let first $\mathbb P(E)\to0$, then $K\to\infty$. Apply this to events involving the supremum on a finite horizon for the uniform-in-probability statement.

Let $\mathcal C$ be the bounded [predictable](../../../../../../predictable-process.md) integrands for which the two integral processes agree up to $\mathbb Q$-indistinguishability. It is a vector space containing elementary rectangle indicators generating the [predictable](../../../../../../predictable-process.md) sigma-algebra. It is closed under uniformly bounded pointwise limits: stochastic [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives convergence of the integrals under each measure, and the preceding transfer makes the $\mathbb P$ limit also a $\mathbb Q$ limit. Uniqueness of limits in probability makes the two limiting integrals equal. The [functional monotone-class theorem](../../../../../../functional-monotone-class-theorem.md) therefore puts every bounded [predictable](../../../../../../predictable-process.md) integrand in $\mathcal C$.

Finally, for locally bounded $H$, stop on intervals where it has a deterministic bound. Such [stopping times](../../../../../../stopping-time.md) tend to infinity under $\mathbb P$ and hence also under $\mathbb Q$. Apply the bounded result to the stopped integrands and use the stopping property of the integral. This proves the [stochastic integral under an absolutely continuous measure change](../../../../../../stochastic-integral-under-an-absolutely-continuous-measure-change.md) identity

$$
\boxed{(H\cdot X)^{\mathbb P}=(H\cdot X)^{\mathbb Q}\quad\mathbb Q\text{-indistinguishably}.}
$$

The decompositions $H\cdot M+H\cdot A$ and $H\cdot N+H\cdot B$ thus represent the same process under $\mathbb Q$, although their individual components need not agree. With only absolute continuity, equality is asserted outside a $\mathbb Q$-null set, not necessarily outside a $\mathbb P$-null set for a chosen $\mathbb Q$ version.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
