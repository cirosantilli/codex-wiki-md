<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take a [random variable](../../../../../../random-variable-split.md) $Z$ with the [Rademacher distribution](../../../../../../rademacher-distribution.md), and set

$$
X_n=Z,\qquad Y_n=\begin{cases}Z,&n\text{ even},\\-Z,&n\text{ odd}.\end{cases}
$$

Both [marginal distributions](../../../../../../marginal-distribution.md) equal the law of $Z$ for every $n$. Hence $X_n$ and $Y_n$ each have [weak convergence of random variables](../../../../../../convergence-in-distribution.md) to $Z$; one may take $X=Y=Z$ on this [probability space](../../../../../../probability-space.md). But their sums alternate:

$$
X_n+Y_n=\begin{cases}2Z,&n\text{ even},\\0,&n\text{ odd}.\end{cases}
$$

Indeed, at $t=\pi/2$ their [characteristic functions](../../../../../../characteristic-function.md) are $-1$ for even $n$ and $1$ for odd $n$, so the sums have no weak limit at all. **Separate marginal weak convergence does not imply convergence of the sum.** The [marginal weak convergence does not control sums](../../../../../../marginal-weak-convergence-does-not-control-sums.md) counterexample changes the dependence while leaving the marginals fixed. Unlike [convergence in probability](../../../../../../convergence-in-probability.md), separate marginal [weak convergence of random variables](../../../../../../convergence-in-distribution.md) contains no information about the joint coupling.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
