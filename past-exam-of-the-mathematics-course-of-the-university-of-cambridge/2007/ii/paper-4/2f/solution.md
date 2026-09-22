<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

The two-dimensional [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) states that every continuous map from a closed filled triangle to itself has a fixed point. Use the triangle $\Delta=\{x\in\mathbb R^3:x_i\geq0,\ \sum_i x_i=1\}$, which lies in a two-dimensional affine plane. Strict positivity of the matrix entries ensures $(Ax)_i>0$ for every $x\in\Delta$. Therefore

$$
T(x)=\frac{Ax}{\sum_i(Ax)_i}
$$

is a continuous self-map of $\Delta$, in fact into its interior. Its fixed point $x$ satisfies $Ax=\lambda x$, where $\lambda=\sum_i(Ax)_i>0$. Since $x=T(x)$ lies in the interior, **$A$ has an [eigenvector](../../../../../eigenvector.md) all of whose entries are strictly positive**. This is [positive matrix eigenvector from simplex normalization](../../../../../positive-matrix-eigenvector-from-simplex-normalization.md); it uses strict positivity, not merely nonnegative entries.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
