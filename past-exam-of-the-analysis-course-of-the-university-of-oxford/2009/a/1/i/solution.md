<h1 id="a/1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [normed vector space](../../../../../normed-vector-space-split.md) is a real or complex [vector space](../../../../../vector-space-split.md) $X$ with a [norm](../../../../../norm.md) satisfying positivity, definiteness, absolute homogeneity and the [triangle inequality](../../../../../triangle-inequality.md). It is [separable](../../../../../separable-topological-space.md) if it has a countable [dense subset](../../../../../dense-set.md) for the [norm](../../../../../norm.md) distance.

First prove the unlabelled general assertions. If $(x_n)$ is dense in $X$, choose $y_{n,m}\in Y\cap B(x_n,1/m)$ whenever that intersection is nonempty. These choices form a countable subset of $Y$. For any $y\in Y$ and $\varepsilon>0$, choose $m$ with $2/m<\varepsilon$ and $n$ with $\|x_n-y\|<1/m$. The corresponding intersection is nonempty and $\|y-y_{n,m}\|<2/m<\varepsilon$. Thus **every subspace of a [separable](../../../../../separable-topological-space.md) [normed vector space](../../../../../normed-vector-space-split.md) is [separable](../../../../../separable-topological-space.md)**.

If a countable $S$ has dense [linear span](../../../../../linear-span.md), take all finite linear combinations of its elements with rational coefficients in the real case, or coefficients in $\mathbb Q+i\mathbb Q$ in the complex case. This set is countable and dense in the [linear span](../../../../../linear-span.md), by approximating the finitely many coefficients of each combination. Its closure is therefore $X$, proving separability. Conversely, a countable dense set already has dense [linear span](../../../../../linear-span.md).

For $c_0$, use all [finitely supported sequences](../../../../../finitely-supported-sequence.md) with coordinates in $\mathbb Q+i\mathbb Q$. Truncate a sequence tending to zero to control its supremum tail, then approximate the finite initial coordinates. This produces a countable [dense subset](../../../../../dense-set.md), so

$$
\boxed{c_0\text{ is separable}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
