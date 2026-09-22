<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the three-bit [majority function](../../../../../../majority-function.md), the pair products count how many pairs of input bits are both one. Their sum is zero at [Hamming weights](../../../../../../hamming-weight.md) zero and one, one at weight two, and three at weight three. Subtracting twice the triple product corrects the last value. Hence

$$
\boxed{\operatorname{MAJ}(x)=x_1x_2+x_1x_3+x_2x_3-2x_1x_2x_3.}
$$

This is a [multilinear polynomial](../../../../../../multilinear-polynomial.md) of degree three, and its top coefficient is nonzero. Uniqueness of the Boolean [multilinear polynomial](../../../../../../multilinear-polynomial.md) excludes a degree-two alternative. The [polynomial method for quantum query lower bounds](../../../../../../polynomial-method-for-quantum-query-lower-bounds.md) therefore yields $T\ge3/2$, and the integer number of queries gives

$$
\boxed{Q_E(\operatorname{MAJ})\ge2.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
