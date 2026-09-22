<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use coordinates in which the current spacing is $h$. On the first child subgrid, the polynomial candidate is

$$
Q_+(x)=\tfrac34P(x-h/4)+\tfrac14P(x+3h/4);
$$

on the second it is

$$
Q_-(x)=\tfrac14P(x-3h/4)+\tfrac34P(x+h/4).
$$

For arbitrary sufficiently long uniformly spaced data, all refined vertices can lie on one degree-$n$ polynomial only if these two candidate polynomials agree. They agree with $P$ when $n=0,1$. For $P(x)=ax^2+bx+c$, expansion gives

$$
Q_+(x)=Q_-(x)=P(x)+\frac{3ah^2}{16}.
$$

Thus quadratics preserve their degree, although not the same values.

For a polynomial of degree $n\geq3$, subtract the two finite Taylor expansions. The first-derivative term cancels, while the leading nonzero differential term is

$$
Q_+(x)-Q_-(x)=\frac{h^3}{32}P^{(3)}(x)+\text{terms involving higher odd derivatives}.
$$

If the leading coefficient of $P$ is $a_n\ne0$, this difference has nonzero coefficient $a_n n(n-1)(n-2)h^3/32$ at degree $n-3$; the higher derivatives have lower degree and cannot cancel it. Therefore the [polynomial degree preservation under Chaikin subdivision](../../../../../../polynomial-degree-preservation-under-chaikin-subdivision.md) holds exactly for

$$
\boxed{n=0,1,2.}
$$

This is a general refinement property, independent of accidental interpolation through a small finite number of vertices.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
