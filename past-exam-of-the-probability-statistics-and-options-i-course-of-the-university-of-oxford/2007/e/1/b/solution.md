<h1 id="e/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [metric space](../../../../../metric-space.md) is sequentially compact if every sequence in it has a [subsequence](../../../../../subsequence.md) converging to a point of the same space. The sequence $x_n=1/(n+1)$ lies in $(0,1)$, but every [subsequence](../../../../../subsequence.md) converges in $\mathbb R$ to zero. Uniqueness of limits excludes an alternative limit inside $(0,1)$, so **the open interval is not sequentially compact**.

For the product, take any sequence $(x_n,y_n)$. [sequential compactness](../../../../../sequentially-compact-space.md) of $X$ gives a [subsequence](../../../../../subsequence.md) $x_{n_k}\to x\in X$. Apply [sequential compactness](../../../../../sequentially-compact-space.md) of $Y$ to the corresponding sequence $y_{n_k}$ to obtain a further [subsequence](../../../../../subsequence.md) $y_{n_{k_j}}\to y\in Y$. Passing to a [subsequence](../../../../../subsequence.md) preserves the convergence of the first coordinate, and therefore

$$
d((x_{n_{k_j}},y_{n_{k_j}}),(x,y))
=d_X(x_{n_{k_j}},x)+d_Y(y_{n_{k_j}},y)\to0.
$$

Thus **$X\times Y$ is sequentially compact** with the stated sum metric. Taking the second coordinate [subsequence](../../../../../subsequence.md) inside the first one is essential; two unrelated [subsequences](../../../../../subsequence.md) would not suffice.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [E](../../../e.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
