<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed disjoint $A,B$, the random variable $e(A,B)$ has the [binomial distribution](../../../../../../binomial-distribution.md) $\operatorname{Bin}(|A||B|,p)$. A two-sided [Chernoff bound](../../../../../../chernoff-bound.md) gives

$$
\mathbb P\bigl(|e(A,B)-p|A||B||>\varepsilon|A||B|\bigr)
\leq2e^{-c_{p,\varepsilon}|A||B|}.
$$

When $|A|,|B|\geq n/\log n$, this is at most

$$
2\exp\left(-c_{p,\varepsilon}\frac{n^2}{(\log n)^2}\right).
$$

There are at most $3^n$ ordered disjoint pairs $(A,B)$, since each vertex can lie in $A$, in $B$, or in neither. The [union bound](../../../../../../boole-s-inequality.md) therefore makes the probability of any failure at most

$$
2\cdot3^n\exp\left(-c_{p,\varepsilon}\frac{n^2}{(\log n)^2}\right)=o(1),
$$

which proves the simultaneous estimate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
