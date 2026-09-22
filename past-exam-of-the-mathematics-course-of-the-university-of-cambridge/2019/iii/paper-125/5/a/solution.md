<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $P=[x_0:\cdots:x_N]\in\mathbb P^N(\mathbb Q)$, choose coprime integer coordinates and define the [projective height](../../../../../../projective-height.md)

$$
H(P)=\max_i|x_i|.
$$

Write the morphism $F:\mathbb P^1\to\mathbb P^1$ as $F=[F_0:F_1]$, where $F_0,F_1\in\mathbb Z[X,Y]$ are homogeneous of degree $d$ with no common zero. Bounding each polynomial by the sum of the absolute values of its coefficients gives

$$
H(F(P))\leq c_2H(P)^d.
$$

Because $F_0$ and $F_1$ have no common projective zero, the [Projective Nullstellensatz](../../../../../../projective-nullstellensatz.md) gives an integer $m\geq d$ and homogeneous polynomials $A_{ij}$ such that suitable nonzero integer multiples of $X^m$ and $Y^m$ lie in the ideal $(F_0,F_1)$. Evaluating at primitive coordinates and using the same coefficient bound gives

$$
H(P)^m\leq C H(P)^{m-d}H(F(P)),
$$

after absorbing the bounded common divisor of $F_0(x,y)$ and $F_1(x,y)$ into $C$. Therefore

$$
\boxed{c_1H(P)^d\leq H(F(P))\leq c_2H(P)^d.}
$$

This is [height growth under a morphism of the projective line](../../../../../../height-growth-under-a-morphism-of-the-projective-line.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
