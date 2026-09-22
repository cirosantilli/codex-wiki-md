<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Taking the [natural logarithm](../../../../../../natural-logarithm.md) of the finite [Euler product](../../../../../../euler-product.md) and using the [Taylor series](../../../../../../taylor-series.md)

$$
-\log(1-u)=u+\sum_{k\geq2}\frac{u^k}{k}
$$

gives

$$
\log\prod_{p\leq x}\left(1-\frac1p\right)^{-1}
=\sum_{p\leq x}\frac1p
+\sum_{p\leq x}\sum_{k\geq2}\frac1{kp^k}.
$$

The double series converges absolutely, and the [Mertens second theorem](../../../../../../mertens-second-theorem.md) therefore makes the right side

$$
\log\log x+\log C+O\left(\frac1{\log x}\right)
$$

for

$$
C=\exp\left(c+\sum_p\sum_{k\geq2}\frac1{kp^k}\right)>0.
$$

Exponentiating proves

$$
\boxed{\prod_{p\leq x}\left(1-\frac1p\right)^{-1}
=C\log x+O(1).}
$$

This is the [Mertens third theorem](../../../../../../mertens-third-theorem.md).

## ↑ Ancestors (11)

1. [D](../d.md)
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
