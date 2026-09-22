<h1 id="9f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [geometric distribution](../../../../../../geometric-distribution.md) with parameter $p$ on $\{1,2,\ldots\}$ has [probability mass function](../../../../../../probability-mass-function.md)

$$
\boxed{P(X=n)=(1-p)^{n-1}p,\qquad n\geq1.}
$$

It counts the trial on which the first success occurs in independent trials with success [probability](../../../../../../probability.md) $p$. Its [probability generating function](../../../../../../probability-generating-function.md) is $ps/[1-(1-p)s]$. Differentiating at $s=1$ gives

$$
EX=\frac1p,\qquad \operatorname{Var}X=\frac{1-p}{p^2}.
$$

This support convention is important: a count of failures before the first success would start at zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
