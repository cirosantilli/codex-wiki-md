<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

We first justify the maximum in the proposed [supremum norm](../../../../../supremum-norm.md). If a [null sequence](../../../../../null-sequence.md) $x$ is nonzero, choose an index $j$ with $|x_j|>0$. All sufficiently late terms have absolute value smaller than $|x_j|/2$, since $x_i\to0$. Hence the largest absolute value occurs among a finite initial set of terms, and is finite. For the zero sequence the maximum is zero.

The [norm](../../../../../norm.md) axioms now follow directly. The maximum is nonnegative and vanishes precisely when every coordinate vanishes. For a scalar $a$, $\|ax\|_\infty=|a|\|x\|_\infty$. For two [null sequences](../../../../../null-sequence.md), coordinatewise addition remains a [null sequence](../../../../../null-sequence.md) and

$$
|x_i+y_i|\leq|x_i|+|y_i|\leq\|x\|_\infty+\|y\|_\infty.
$$

Taking the maximum proves the [triangle inequality](../../../../../triangle-inequality.md), so this really is a [norm](../../../../../norm.md) on $V$.

Let $e_n$ have a single $1$ in position $n$. If $m\ne n$, then $\|e_m-e_n\|_\infty=1$. A convergent sequence in a [normed vector space](../../../../../normed-vector-space.md) must be a [Cauchy sequence](../../../../../cauchy-sequence.md), by the [triangle inequality](../../../../../triangle-inequality.md). These distances violate the Cauchy condition with, for example, $\varepsilon=1/2$. Thus **$(e_n)$ does not converge in this norm**, even though each fixed coordinate converges to zero.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
