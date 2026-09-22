<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

[Independence of random variables](../../../../../independent-random-variables.md) and the two unit-rate [exponential distributions](../../../../../exponential-distribution.md) give

$$
f_{X,Y}(x,y)=e^{-x-y}\mathbf1_{\{x\geq0,\ y\geq0\}}.
$$

The [linear transformation](../../../../../linear-map.md)

$$
\begin{pmatrix}U\\V\end{pmatrix}
=\begin{pmatrix}6&8\\2&3\end{pmatrix}
\begin{pmatrix}X\\Y\end{pmatrix}
$$

has determinant $2$ and inverse

$$
x=\frac{3u-8v}{2},\qquad y=-u+3v.
$$

The inequalities $x,y\geq0$ become $8v/3\leq u\leq3v$. By the [change-of-variables formula for probability densities](../../../../../change-of-variables-formula-for-a-probability-density.md),

$$
\boxed{f_{U,V}(u,v)=\frac12e^{-u/2+v}\mathbf1_{\{v\geq0,\ 8v/3\leq u\leq3v\}}}.
$$

The variables $U$ and $V$ are not independent: the support of their joint density is a wedge rather than a [Cartesian product](../../../../../cartesian-product.md) of one-dimensional supports. For example, conditioning on a positive value of $V$ constrains $U$ to a finite interval depending on that value.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
