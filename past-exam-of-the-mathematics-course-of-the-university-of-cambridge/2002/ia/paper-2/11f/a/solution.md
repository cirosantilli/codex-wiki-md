<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [independent random variables](../../../../../../independent-random-variables.md), the [probability density function](../../../../../../probability-density-function.md) of a sum is the [convolution of probability densities](../../../../../../convolution-of-independent-random-variables.md). Since each density is one on $[0,1]$ and zero elsewhere,

$$
f_{X+Y}(u)=\int_{\mathbb R}\mathbf1_{[0,1]}(x)\mathbf1_{[0,1]}(u-x)\,dx.
$$

This is the length of $[0,1]\cap[u-1,u]$. Therefore **the density is**

$$
\boxed{f_{X+Y}(u)=\begin{cases}u&0\le u\le1,\\2-u&1\le u\le2,\\0&\text{otherwise}.\end{cases}}
$$

The two triangular areas sum to one, as a [probability density function](../../../../../../probability-density-function.md) must.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
