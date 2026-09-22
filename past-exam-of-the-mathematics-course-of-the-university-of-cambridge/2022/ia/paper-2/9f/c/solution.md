<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The normalizing constant satisfies

$$
B^{-1}=\sum_{n\in\mathbb Z}e^{-n^2/2}.
$$

For an integer $k$,

$$
\mathbb E[e^{kY}]
=B\sum_{n\in\mathbb Z}e^{kn-n^2/2}
=Be^{k^2/2}\sum_{n\in\mathbb Z}e^{-(n-k)^2/2}.
$$

Translation by the integer $k$ merely permutes the summation indices, so the final sum is $B^{-1}$. Consequently

$$
\boxed{\mathbb E[e^{kY}]=e^{k^2/2}
=\mathbb E[e^{kX}]}.
$$

The last equality uses the [moment-generating function](../../../../../../moment-generating-function.md) of the standard normal variable from part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
