<h1 id="11f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If exactly $k$ spins equal $+1$, then $M=(2k-n)/n$. Therefore its possible values are $E_n$, with $k=n(1+m)/2$ for $m\in E_n$. Choosing the $k$ positive spins gives the [binomial coefficient](../../../../../../binomial-coefficient.md)

$$
\binom nk=\frac{n!}{[n(1+m)/2]!\,[n(1-m)/2]!}.
$$

Every such configuration has the same [Curie–Weiss model](../../../../../../curie-weiss-model.md) weight because $\sum_{i,j}s_is_j=(\sum_is_i)^2=n^2m^2$. The [probability mass function](../../../../../../probability-mass-function.md) of this [spin magnetization](../../../../../../spin-magnetization.md) is consequently

$$
\boxed{\mathbb P(M=m)=\frac1{Z_{n,\beta}}
\binom{n}{n(1+m)/2}e^{\beta nm^2/2},\qquad m\in E_n,}
$$

and zero elsewhere. Grouping the original [partition function](../../../../../../canonical-partition-function.md) by the same count also gives

$$
Z_{n,\beta}=\sum_{k=0}^n\binom nk
\exp\!\left[\frac{\beta(2k-n)^2}{2n}\right],
$$

which verifies normalization without counting any configuration twice.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
