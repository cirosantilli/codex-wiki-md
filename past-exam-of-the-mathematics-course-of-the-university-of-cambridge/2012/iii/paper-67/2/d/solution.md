<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Boolean conjunction is multiplication on zero-one inputs. The [block conjunction of three-bit majorities](../../../../../../block-conjunction-of-three-bit-majorities.md) therefore has the [multilinear polynomial](../../../../../../multilinear-polynomial.md)

$$
P_n(x)=\prod_{i=1}^n\left(x_{3i-2}x_{3i-1}+x_{3i-2}x_{3i}+x_{3i-1}x_{3i}-2x_{3i-2}x_{3i-1}x_{3i}\right).
$$

The factors use disjoint variables, so their product remains a [multilinear polynomial](../../../../../../multilinear-polynomial.md). Its monomial containing all $3n$ variables has coefficient $(-2)^n\ne0$; no term has higher degree. By uniqueness, the representing [multilinear polynomial](../../../../../../multilinear-polynomial.md) has degree exactly $3n$. Applying the [polynomial method for quantum query lower bounds](../../../../../../polynomial-method-for-quantum-query-lower-bounds.md) gives

$$
\boxed{Q_E(\operatorname{MAJ}_n)\ge\left\lceil\frac{3n}{2}\right\rceil.}
$$

This argument concerns [exact quantum query complexity](../../../../../../exact-quantum-query-complexity.md); the analogous claim for bounded error does not follow from exact polynomial degree.

## ↑ Ancestors (11)

1. [D](../d.md)
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
