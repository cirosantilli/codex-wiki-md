<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

For a partition $P$, write $U(f,P)$ and $L(f,P)$ for the [upper Darboux sum](../../../../../upper-darboux-sum.md) and [lower Darboux sum](../../../../../lower-darboux-sum.md). The [Riemann integrability criterion](../../../../../riemann-integrability-criterion.md) for bounded $f$ is that for every $\varepsilon>0$ some partition satisfies $U(f,P)-L(f,P)<\varepsilon$. Thus if the gaps for $D_n$ tend to zero, the [Riemann integrability criterion](../../../../../riemann-integrability-criterion.md) immediately proves that $f$ is [Riemann integrable](../../../../../riemann-integrable-function.md).

Conversely, suppose $f$ is [Riemann integrable](../../../../../riemann-integrable-function.md), and choose a fixed partition $P$ with $U(f,P)-L(f,P)<\varepsilon/2$. Let $r$ be the number of its interior division points and choose $M\geq1$ with $|f|\leq M$. Call a cell of $D_n$ bad when its interior contains a division point of $P$. There are at most $r$ bad cells, and their total length is at most $r/n$.

Every other cell lies in a single cell of $P$, so its oscillation is no larger than that of the containing cell. Summing the contributions of these good cells gives at most $U(f,P)-L(f,P)$, while each bad cell has oscillation at most $2M$. Therefore the [finite bad-cell estimate for Darboux sums](../../../../../finite-bad-cell-estimate-for-darboux-sums.md) gives

$$
0\leq U(f,D_n)-L(f,D_n)\leq U(f,P)-L(f,P)+\frac{2Mr}{n}.
$$

For large enough $n$, the right-hand side is less than $\varepsilon$. This proves the [uniform-mesh Darboux criterion](../../../../../uniform-mesh-darboux-criterion.md)

$$
\boxed{f\text{ is Riemann integrable}\quad\Longleftrightarrow\quad U(f,D_n)-L(f,D_n)\longrightarrow0.}
$$

This argument does not assume that the partitions $D_n$ are nested; in general they are not.

For the composition, $f$ takes values in $[-M,M]$. Since $g$ is continuously differentiable, the [extreme value theorem](../../../../../extreme-value-theorem.md) bounds both $|g|$ and $|g'|$ on that interval. In particular, let $K=\sup_{[-M,M]}|g'|<\infty$. The [mean value theorem](../../../../../mean-value-theorem.md) states that a function continuous on the interval between $s,t$ and differentiable in its interior satisfies $g(s)-g(t)=g'(\xi)(s-t)$ for some intermediate $\xi$. Hence

$$
|g(s)-g(t)|\leq K|s-t|\qquad(s,t\in[-M,M]).
$$

On each partition cell, this bounds the oscillation of $g\circ f$ by $K$ times the oscillation of $f$, whether or not the local extrema are attained. It follows that

$$
U(g\circ f,D_n)-L(g\circ f,D_n)\leq K\bigl(U(f,D_n)-L(f,D_n)\bigr)\longrightarrow0.
$$

The composition is bounded, so the proved [uniform-mesh Darboux criterion](../../../../../uniform-mesh-darboux-criterion.md) applies. Thus **$g\circ f$ is Riemann integrable**. The reusable fact is [Lipschitz composition preserves Riemann integrability](../../../../../lipschitz-composition-preserves-riemann-integrability.md); continuous differentiability supplies the required bound on the range of $f$.

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
