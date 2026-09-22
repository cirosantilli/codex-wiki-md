<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [probability generating function](../../../../../../probability-generating-function.md) is

$$
G_X(s)=\sum_{m=1}^{\infty}\mathbb P(X=m)s^m.
$$

Differentiating $n$ times,

$$
G_X^{(n)}(s)
=\sum_{m=n}^{\infty}
\frac{m!}{(m-n)!}\mathbb P(X=m)s^{m-n}.
$$

At $s=0$, only the term $m=n$ remains. Hence

$$
\boxed{\mathbb P(X=n)=\frac{G_X^{(n)}(0)}{n!}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
