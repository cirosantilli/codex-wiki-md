<h1 id="10i/solution">Solution</h1>

↑ **Parent:** [10I](../10i.md)

Work in the complete [Banach space](../../../../../banach-space-split.md) $C([0,1])$ with the [uniform norm](../../../../../supremum-norm.md). Each $E_m$ is closed. Indeed if $f_j\to f$ uniformly and $x_j$ witnesses membership in $E_m$, pass to a subsequence with $x_j\to x$. For each $y\in[0,1]$, uniform convergence and continuity give

$$
|f(y)-f(x)|=\lim_j|f_j(y)-f_j(x_j)|\leq m|y-x|^\alpha.
$$

Thus $x$ witnesses membership for $f$.

Each $E_m$ has empty interior. Approximate an arbitrary $f$ uniformly by a [piecewise linear function](../../../../../piecewise-linear-function.md) $q$ on a uniform mesh, and let $D$ bound the absolute slopes of $q$. On a sufficiently fine uniform refinement of mesh $\delta$, add a triangular oscillation of fixed small amplitude $b$, alternating between $b$ and $-b$ at successive vertices. The resulting function $g$ is still as close to $f$ as desired, and every segment has absolute slope at least $2b/\delta-D$. For any $x$, choose the farther endpoint of a segment containing $x$. Its distance $h$ is between $\delta/2$ and $\delta$, so

$$
\frac{|g(x+h)-g(x)|}{|h|^\alpha}\geq (2b/\delta-D)\delta^{1-\alpha}\min(1,2^{\alpha-1})>m
$$

when $\delta$ is small. Therefore $g\notin E_m$.

By the [Baire category theorem](../../../../../baire-category-theorem.md), the complement of $\bigcup_m E_m$ is dense and nonempty. If the local limsup in the question were finite at some $x$, its nearby differences would satisfy a finite bound. The remaining differences, with $|h|\geq\delta>0$, are bounded by $2\|f\|_\infty\delta^{-\alpha}$. Combining the bounds would put $f$ in some $E_m$, a contradiction. Hence **the required limsup is infinite at every point**, including one-sided approaches at the endpoints.

## ↑ Ancestors (10)

1. [10I](../10i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
