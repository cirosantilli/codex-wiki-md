<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the coordinatewise [partial order](../../../../../partially-ordered-set.md): $\omega\leq\eta$ means $\omega(e)\leq\eta(e)$ for every $e\in E$. An [increasing event](../../../../../increasing-event.md) $A$ is upward closed: $\omega\in A$ and $\omega\leq\eta$ imply $\eta\in A$.

Under the independent [Bernoulli distribution](../../../../../bernoulli-distribution.md) [product measure](../../../../../product-measure.md) $\mathbb P_p$ on these coordinates, the [Harris-FKG inequality](../../../../../harris-fkg-inequality.md) states

$$
\boxed{\mathbb P_p(A\cap B)\geq\mathbb P_p(A)\mathbb P_p(B)}
$$

for [increasing events](../../../../../increasing-event.md) $A,B$. For $K\subseteq E$, let $[\omega]_K$ be the cylinder of configurations agreeing with $\omega$ on $K$. The [disjoint occurrence of increasing events](../../../../../disjoint-occurrence-of-increasing-events.md) $A\square B$ consists of configurations for which there exist disjoint $K,L$ with $[\omega]_K\subseteq A$ and $[\omega]_L\subseteq B$. For [increasing events](../../../../../increasing-event.md), witnesses can be taken to prescribe only open coordinates. The [BK inequality](../../../../../van-den-berg-kesten-inequality.md) is

$$
\boxed{\mathbb P_p(A\square B)\leq\mathbb P_p(A)\mathbb P_p(B).}
$$

Positive association rewards simultaneous occurrence; the disjoint-witness requirement in the [BK inequality](../../../../../van-den-berg-kesten-inequality.md) gives a bound in the opposite direction. The inequalities also apply to different independent Bernoulli parameters in different coordinates.

Regard the boxes as sets of lattice [graph vertices](../../../../../vertex-graph-theory.md). Write $\tau_p(x,y)=\mathbb P_p(x\leftrightarrow y)$, and put $g_0=1$. On the event defining $g_n$, choose an open [self-avoiding walk](../../../../../self-avoiding-walk.md) from the origin to its first visit to $\partial\Lambda_n$. Let $y$ be its first visit to $\partial\Lambda_m$. Its initial segment witnesses $0\leftrightarrow y$. Its remaining segment ends at a point $z$ with

$$
\|z-y\|_\infty\geq\|z\|_\infty-\|y\|_\infty=n-m.
$$

For $m<n$, truncate this remaining segment on its first visit to $y+\partial\Lambda_{n-m}$. The two segments use disjoint [edges](../../../../../edge-of-a-graph.md), so they are disjoint witnesses. For $m=n$, the second event is the sure event with empty witness. Thus the [union bound](../../../../../boole-s-inequality.md), the [BK inequality](../../../../../van-den-berg-kesten-inequality.md) and translation invariance give

$$
\begin{aligned}
g_n&\leq\sum_{y\in\partial\Lambda_m}
\mathbb P_p\bigl(\{0\leftrightarrow y\}\square
\{y\leftrightarrow y+\partial\Lambda_{n-m}\}\bigr)\\
&\leq\boxed{g_{n-m}\sum_{y\in\partial\Lambda_m}\tau_p(0,y)}.
\end{aligned}
$$

An unrestricted connection event can depend on infinitely many [edges](../../../../../edge-of-a-graph.md). Apply the finite-coordinate [BK inequality](../../../../../van-den-berg-kesten-inequality.md) first to connections confined to growing boxes and take increasing limits; each occurrence has a finite path witness. This justifies its use here. The estimate is the [weighted BK boundary-splitting estimate](../../../../../weighted-bk-boundary-splitting-estimate.md).

By summing cluster indicators and using [Tonelli theorem](../../../../../tonelli-theorem.md), the [percolation susceptibility](../../../../../percolation-susceptibility.md) is

$$
\chi(p)=\mathbb E_p|C(0)|=\sum_{y\in\mathbb Z^d}\tau_p(0,y)
=1+\sum_{m\geq1}S_m,\qquad
S_m=\sum_{y\in\partial\Lambda_m}\tau_p(0,y).
$$

If $\chi(p)<\infty$, then $S_m\to0$. At $p=0$ all $g_k$ vanish, so any positive exponential rate works. Otherwise choose $m\geq1$ with $a=S_m\in(0,1)$. Iterating the [weighted BK boundary-splitting estimate](../../../../../weighted-bk-boundary-splitting-estimate.md) gives, for $k=jm+r$ with $0\leq r<m$,

$$
g_k\leq a^j g_r\leq a^{\lfloor k/m\rfloor}.
$$

For $k\geq m$, $\lfloor k/m\rfloor\geq k/(2m)$, so $g_k\leq\exp[-(-\log a)k/(2m)]$. To include the finitely many smaller indices without a prefactor, note that $p<1$ under finite susceptibility and

$$
g_k\leq g_1=1-(1-p)^{2d}<1\qquad(k\geq1).
$$

Therefore one may take

$$
\boxed{\mu(p)=\min\left\{\frac{-\log a}{2m},
\frac{-\log g_1}{m}\right\}>0,\qquad
 g_k\leq e^{-\mu(p)k}\quad(k\geq1).}
$$

For $k<m$ this follows from $\mu(p)k\leq-\log g_1$, and for $k\geq m$ it follows from the iterated estimate. This proves [exponential one-arm decay from finite susceptibility](../../../../../exponential-one-arm-decay-from-finite-susceptibility.md) with exactly the requested unit prefactor.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
