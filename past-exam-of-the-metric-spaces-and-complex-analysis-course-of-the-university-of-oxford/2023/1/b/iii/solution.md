<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

Let $(F_n)$ be a [Cauchy sequence](../../../../../cauchy-sequence.md) for the [Hausdorff distance](../../../../../hausdorff-distance.md), and put

$$
\delta_n=\sup_{p,q\geq n}\rho(F_p,F_q),\qquad A_n=\overline{\bigcup_{m\geq n}F_m}.
$$

The [bounded set](../../../../../bounded-set.md) hypothesis makes $\delta_n$ finite, and the [Cauchy sequence](../../../../../cauchy-sequence.md) property gives $\delta_n\to0$. Each $A_n$ is nonempty and a [closed set](../../../../../closed-set.md), with $A_{n+1}\subseteq A_n$.

We need estimates that survive taking the [closure](../../../../../closure-topology.md). For every nonempty $F$, the [distance to a set](../../../../../distance-to-a-set.md) is [Lipschitz continuous](../../../../../lipschitz-continuity.md) with constant one: the [triangle inequality](../../../../../triangle-inequality.md) gives $\operatorname{dist}(x,F)\leq d(x,y)+\operatorname{dist}(y,F)$, and interchanging $x,y$ proves

$$
|\operatorname{dist}(x,F)-\operatorname{dist}(y,F)|\leq d(x,y).
$$

For every $m\geq n$, points of $F_m$ have distance at most $\delta_n$ from $F_n$. The same holds throughout their union and its [closure](../../../../../closure-topology.md), by this [continuity](../../../../../continuous-function.md). Since $F_n\subseteq A_n$,

$$
\rho(F_n,A_n)\leq\delta_n.
$$

More generally, if $m\geq n$, every point in $\bigcup_{k\geq n}F_k$ is within $\delta_n$ of $F_m\subseteq A_m$. Passing to its [closure](../../../../../closure-topology.md) again, and using $A_m\subseteq A_n$, gives

$$
\rho(A_n,A_m)\leq\delta_n.
$$

Choose strictly increasing indices $n_j$ with $\delta_{n_j}\leq2^{-j}$. Then $(A_{n_j})$ satisfies part (ii), so it converges in [Hausdorff distance](../../../../../hausdorff-distance.md) to the nonempty [closed set](../../../../../closed-set.md) $G=\bigcap_j A_{n_j}=\bigcap_n A_n$, with $\rho(A_{n_j},G)\leq2^{1-j}$.

For $n\geq n_j$, the [triangle inequality](../../../../../triangle-inequality.md) gives the explicit full-sequence bound

$$
\rho(F_n,G)\leq\rho(F_n,F_{n_j})+\rho(F_{n_j},A_{n_j})+\rho(A_{n_j},G)
\leq2\delta_{n_j}+2^{1-j}\leq2^{2-j}.
$$

It tends to zero as $j\to\infty$. Therefore

$$
\boxed{X\text{ complete}\ \Longrightarrow\ (\mathcal F(X),\rho)\text{ complete}}.
$$

This proves [Completeness of the Hausdorff hyperspace](../../../../../completeness-of-the-hausdorff-hyperspace.md) using the proposed tail closures, rather than assuming their diameters shrink.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [b](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
