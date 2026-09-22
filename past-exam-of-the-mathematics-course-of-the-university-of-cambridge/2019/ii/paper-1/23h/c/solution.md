<h1 id="23h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Equip $\mathbb N$ with [counting measure](../../../../../../counting-measure.md) $\#$. For a nonnegative function $f:\mathbb N\to[0,\infty]$, define

$$
\boxed{\sum_{n\geq1}f(n)
:=\int_{\mathbb N}f\,d\#
=\sup_{N\geq1}\sum_{n=1}^Nf(n)}.
$$

This lies in $[0,\infty]$ and agrees with the [series as a Lebesgue integral against counting measure](../../../../../../series-as-a-lebesgue-integral-against-counting-measure.md).

For $f:\mathbb N\to\mathbb C$, define

$$
\sum_{n\geq1}f(n)=\int_{\mathbb N}f\,d\#
$$

when $f$ is integrable, which here means

$$
\boxed{\sum_{n\geq1}|f(n)|<\infty}.
$$

Thus the complex sum is defined under [absolute convergence](../../../../../../absolute-convergence.md) and can be obtained by integrating the real and imaginary parts.

A [simple function](../../../../../../simple-function.md) on $\mathbb N$ is a function with finite range, equivalently

$$
s=\sum_{j=1}^ma_j\mathbf1_{A_j}
$$

for a finite measurable partition by subsets $A_j\subseteq\mathbb N$. Its nonnegative sum is $\sum_ja_j\#A_j$. It is finite exactly when every level set with $a_j>0$ is finite, equivalently when $s$ has finite support after its zero level is discarded.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [23H](../../23h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
