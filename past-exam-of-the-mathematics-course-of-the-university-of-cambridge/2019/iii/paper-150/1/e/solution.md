<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The prime-factor formula for the [Euler totient function](../../../../../../euler-totient-function.md) is

$$
\frac n{\varphi(n)}
=\prod_{p\mid n}\left(1-\frac1p\right)^{-1}.
$$

Let

$$
y=\frac{\log n}{\sqrt{\log\log n}}.
$$

The factors with $p\leq y$ contribute at most

$$
\prod_{p\leq y}\left(1-\frac1p\right)^{-1}
=C\log y+O(1)
=(C+o(1))\log\log n
$$

by the [Mertens third theorem](../../../../../../mertens-third-theorem.md). For $p>y$, the number of distinct prime divisors of $n$ is at most $\log n/\log y$, and hence

$$
\begin{aligned}
\log\prod_{\substack{p\mid n\\p>y}}\left(1-\frac1p\right)^{-1}
&\ll\sum_{\substack{p\mid n\\p>y}}\frac1p\\
&\leq\frac{\log n}{y\log y}
=O\left(\frac1{\sqrt{\log\log n}}\right).
\end{aligned}
$$

Thus the large-prime product is $1+o(1)$, and

$$
\frac n{\varphi(n)}\leq(C+o(1))\log\log n.
$$

Taking reciprocals gives, uniformly as $n\to\infty$,

$$
\boxed{\varphi(n)\geq\left(C^{-1}+o(1)\right)
\frac n{\log\log n}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
