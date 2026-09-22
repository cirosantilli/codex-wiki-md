<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In one proposal of [rejection sampling](../../../../../../rejection-sampling.md), the probability of both proposing a value in $dx$ and accepting it is

$$
h(x)\,dx\,\frac{f(x)}{Mh(x)}
=\frac1M f(x)\,dx.
$$

Integrating shows that the acceptance probability is $1/M$. Conditional on acceptance, the density of the proposed value is therefore

$$
\frac{f(x)/M}{1/M}=f(x).
$$

Each unsuccessful proposal restarts independently, so the eventual output $Y$ has the same conditional density:

$$
\boxed{Y\sim f}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
