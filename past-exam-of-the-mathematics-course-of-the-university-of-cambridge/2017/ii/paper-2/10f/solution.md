<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

The [Baire category theorem](../../../../../baire-category-theorem.md) says that in a nonempty [complete metric space](../../../../../complete-metric-space.md), every countable intersection of open dense sets is dense. To prove it, start in an arbitrary nonempty [open set](../../../../../open-set.md) $O$ and let $G_n$ be open dense. Inductively choose closed balls $\overline B(x_n,r_n)$ with $0<r_n\leq2^{-n}$, contained in $G_n$ and in the interior of the previous ball, with the first also contained in $O$. Density provides a point at each stage, and openness permits the smaller closed ball. The centers are a [Cauchy sequence](../../../../../cauchy-sequence.md); [completeness](../../../../../completeness.md) supplies a [limit](../../../../../limit-of-a-function.md) lying in every closed ball, hence in $O\cap\bigcap_nG_n$. The proof also works at isolated points, where sufficiently small balls are singletons.

The incomplete [metric space](../../../../../metric-space.md) $\mathbb Q$ is a counterexample: it is the countable union of its closed nowhere dense singletons, so the complements are open dense with empty intersection.

For the sequence in the problem, put

$$
E_N=\bigcap_{n,m\geq N}\{x\in[0,1]:|f_n(x)-f_m(x)|\leq\epsilon\}.
$$

Each $E_N$ is closed by [continuity](../../../../../continuous-function.md). [Pointwise convergence](../../../../../pointwise-convergence.md) makes each point's values a [Cauchy sequence](../../../../../cauchy-sequence.md), so $[0,1]=\bigcup_NE_N$. By the [Baire category theorem](../../../../../baire-category-theorem.md), one $E_N$ has nonempty relative interior, which contains a nonempty open interval $J$ in $(0,1)$. This proves the required common tail bound.

If [continuous](../../../../../continuous-function.md) $g_n$ converged pointwise to the rationality indicator, take $\epsilon=1/4$ and let $m\to\infty$ in this bound. On $J$, $|g_n-g|\leq1/4$ for $n\geq N$. Hence a fixed [continuous](../../../../../continuous-function.md) $g_N$ is at least $3/4$ at every rational point and at most $1/4$ at every irrational point of $J$. The density of both sets contradicts [continuity](../../../../../continuous-function.md). Thus **the rationality indicator is not a pointwise [limit](../../../../../limit-of-a-function.md) of [continuous](../../../../../continuous-function.md) functions**.

Nevertheless $h_n(x)=x^n$ are [continuous](../../../../../continuous-function.md) and converge pointwise to $h(x)=0$ for $x<1$, $h(1)=1$. This [limit](../../../../../limit-of-a-function.md) is discontinuous at $1$: **a pointwise [limit](../../../../../limit-of-a-function.md) of [continuous](../../../../../continuous-function.md) functions can be discontinuous**.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
