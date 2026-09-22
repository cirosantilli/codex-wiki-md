<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p$ be the [best uniform approximation](../../../../../../best-uniform-approximation.md) to the [exponential function](../../../../../../exponential-function.md) from the degree-at-most-$n-1$ [polynomial](../../../../../../polynomial-split.md) space. Suppose that $E_{n-1}(e^x)=E_n(e^x)$. Then the same $p$ is best in the larger space. Its error $g(x)=e^x-p(x)$ is nonzero, since the exponential is not a [polynomial](../../../../../../polynomial-split.md). The [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) supplies $n+2$ ordered points where $g$ has alternating signs. By the [intermediate value theorem](../../../../../../intermediate-value-theorem.md), $g$ has at least one zero in each of the $n+1$ intervening intervals, hence at least $n+1$ distinct zeros.

Applying [Rolle's theorem](../../../../../../rolle-theorem.md) successively $n$ times forces a zero of $g^{(n)}$. But $\deg p\le n-1$, so

$$
g^{(n)}(x)=e^x>0
$$

everywhere. This is a contradiction. Together with the automatic non-increase of best errors, it proves

$$
\boxed{E_{n-1}(e^x)>E_n(e^x),\qquad n\ge1.}
$$

The argument is an instance of [strict polynomial error decrease from nonvanishing derivatives](../../../../../../strict-polynomial-error-decrease-from-nonvanishing-derivatives.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
