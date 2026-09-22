<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

The first series is [telescoping](../../../../../telescoping-series.md), since

$$
\frac1{n^2+n}=\frac1n-\frac1{n+1}.
$$

Its $N$th partial sum is $1-1/(N+1)$, so

$$
\boxed{\sum_{n=1}^{\infty}\frac1{n^2+n}=1},
$$

a [rational number](../../../../../rational-number.md).

The second series converges absolutely, for example by the [ratio test](../../../../../ratio-test.md), and is the odd part of the [exponential series](../../../../../exponential-series.md):

$$
\sum_{n=1}^{\infty}\frac1{(2n-1)!}
=\sum_{k=0}^{\infty}\frac1{(2k+1)!}
=\sinh1=\frac{e-e^{-1}}2.
$$

This value is irrational. Indeed, if $a=\sinh1$ were algebraic, then $e$ would satisfy

$$
e^2-2ae-1=0,
$$

making $e$ algebraic over the algebraic numbers and hence algebraic, contrary to the [Hermite theorem on the transcendence of e](../../../../../hermite-theorem-on-the-transcendence-of-e.md). Thus the second sum is in fact [transcendental](../../../../../transcendental-number.md).

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
