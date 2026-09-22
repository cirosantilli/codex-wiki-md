<h1 id="1/a/ii/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The answers are

$$
\boxed{\text{yes, no, yes, yes}.}
$$

Write $M_n(f,g)=\sup_{0\leq t\leq n}|f(t)-g(t)|$. The given [metric](../../../../../../metric.md) describes [locally uniform convergence](../../../../../../locally-uniform-convergence.md): $d(f_j,f)\to0$ if and only if $M_n(f_j,f)\to0$ for every fixed $n$. Indeed,

$$
2^{-n}\min\{M_n(f_j,f),1\}\leq d(f_j,f),
$$

so convergence in $d$ forces $M_n\to0$. Conversely, split the defining [series](../../../../../../series-mathematics.md) at $N$: its tail is at most $\sum_{n>N}2^{-n}=2^{-N}$, and its finitely many initial terms tend to zero.

If $(f_j)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md) in $d$, the same single-term estimate makes it a [Cauchy sequence](../../../../../../cauchy-sequence.md) in the [supremum norm](../../../../../../supremum-norm.md) on every $[0,n]$. The [completeness of the continuous-map space in the uniform metric](../../../../../../completeness-of-the-continuous-map-space-in-the-uniform-metric.md) gives a [continuous function](../../../../../../continuous-function.md) $F_n$ on $[0,n]$ with $f_j\to F_n$ uniformly there. Uniqueness of the [limit of a sequence](../../../../../../limit-of-a-sequence.md) gives $F_{n+1}|_{[0,n]}=F_n$, so these [functions](../../../../../../function-split.md) define a single [continuous function](../../../../../../continuous-function.md) $f$ on $[0,\infty)$. The preceding finite-head and tail argument proves $d(f_j,f)\to0$. Thus the space is [complete](../../../../../../completeness.md).

The constant [functions](../../../../../../function-split.md) $f_j(t)=j$ have $d(f_j,f_k)=1$ whenever $j\ne k$. They have no [convergent subsequence](../../../../../../convergent-subsequence.md), so the space is not [sequentially compact](../../../../../../sequentially-compact-space.md).

For fixed $f,g$, set $\gamma(s)=(1-s)f+sg$. On $[0,n]$,

$$
M_n(\gamma(s),\gamma(s'))=|s-s'|M_n(f,g)\longrightarrow0
$$

as $s'\to s$. The equivalence with [locally uniform convergence](../../../../../../locally-uniform-convergence.md) proves that $\gamma$ is a [continuous path](../../../../../../continuous-path.md) for $d$. Hence the space is [path-connected](../../../../../../path-connected-space.md) and [connected](../../../../../../connected-space.md).

## ↑ Ancestors (14)

1. [3](../3.md)
2. [ii](../../ii.md)
3. [a](../../../a.md)
4. [1](../../../../1.md)
5. [2021](../../../../../2021-split.md)
6. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../../split.md)
7. [Metric spaces and complex analysis course of the University of Oxford](../../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
