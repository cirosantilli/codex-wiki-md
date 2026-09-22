<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $\rho$ be the [cyclic logarithmic coloring](../../../../../../cyclic-logarithmic-coloring.md) from part (iii). Define a [finite coloring](../../../../../../finite-coloring.md) of the [positive integers](../../../../../../positive-integer.md) by

$$
\chi(n)=\rho(\log_2 n)\quad(n\geq2),\qquad \chi(1)=0.
$$

The inner [logarithm](../../../../../../logarithm.md) is at least $1$ whenever $n\geq2$, so this is defined everywhere. Suppose an increasing infinite [sequence](../../../../../../sequence.md) $(x_i)$ made every product with distinct indices [monochromatic](../../../../../../monochromatic-set.md). Fix an index $i$ with $x_i\geq2$ and write $a=\log_2 x_i>0$. The [sequence](../../../../../../sequence.md) is unbounded, so choose $j>i$ with $b=\log_2 x_j\geq28a$. Both ordered products are among the supposedly [monochromatic](../../../../../../monochromatic-set.md) values, but their [logarithms](../../../../../../logarithm.md) satisfy

$$
\frac{\log_2(x_i x_j^2)}{\log_2(x_j x_i^2)}
=\frac{a+2b}{2a+b},\qquad
\boxed{1.9\leq\frac{a+2b}{2a+b}<2.}
$$

Indeed, the first inequality is equivalent to $b\geq28a$, and the second uses $a>0$. Part (iii) therefore gives $\chi(x_i x_j^2)\ne\chi(x_j x_i^2)$, a contradiction. Thus **the assertion with all distinct ordered indices is false**. The obstruction needs an infinite unbounded [sequence](../../../../../../sequence.md); it does not assert that every pair of different [positive integers](../../../../../../positive-integer.md) gives different colors.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
