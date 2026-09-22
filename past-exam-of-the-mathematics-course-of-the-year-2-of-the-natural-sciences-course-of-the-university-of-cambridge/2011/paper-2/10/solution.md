<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

A [group homomorphism](../../../../group-homomorphism.md) $D:G_1\to G_2$ satisfies $D(gh)=D(g)D(h)$ for all $g,h\in G_1$. Its [group kernel](../../../../kernel-of-a-group-homomorphism.md) is

$$
\ker D=\{g\in G_1:D(g)=e_{G_2}\}.
$$

For the matrices, put $X=R(x)$, $Y=R(y)$ and $z=e^{2\pi i/3}$. Since $z^3=1$, $z\ne1$ and $1+z+z^2=0$, direct [matrix multiplication](../../../../matrix-multiplication.md) gives

$$
X^2=I_2,\qquad Y^2=\begin{pmatrix}z^2&0\\0&z\end{pmatrix},\qquad Y^3=I_2,
$$



$$
XY=\begin{pmatrix}0&z^2\\z&0\end{pmatrix},\qquad
XY^2=\begin{pmatrix}0&z\\z^2&0\end{pmatrix}=YX,\qquad
Y^2X=XY.
$$

These verify the listed matrices and the defining relations, with $R(e)=I_2$. To check every product explicitly through a single calculation, write elements in the unique form $x^\epsilon y^j$, with $\epsilon=0,1$ and $j=0,1,2$. The relations give

$$
(x^\epsilon y^j)(x^\eta y^k)=x^{\epsilon+\eta}y^{(-1)^\eta j+k}.
$$

The displayed matrices obey $Y^jX=XY^{-j}$, so their product has exactly the same form:

$$
(X^\epsilon Y^j)(X^\eta Y^k)=X^{\epsilon+\eta}Y^{(-1)^\eta j+k}=R\big((x^\epsilon y^j)(x^\eta y^k)\big).
$$

All exponents are reduced modulo two or three respectively. Thus this verifies all 36 products, and $R$ is a two-dimensional complex [group representation](../../../../group-representation.md). It is given to be an [irreducible representation](../../../../irreducible-representation.md).

For a one-dimensional complex [group representation](../../../../group-representation.md) $U$, let $u=U(x)$ and $v=U(y)$, which are nonzero complex numbers. The relations require

$$
u^2=1,\qquad v^3=1,\qquad vu=uv^2.
$$

Since scalar multiplication commutes and $u\ne0$, the last relation gives $v=v^2$, hence $v=1$. Then $u=\pm1$. The choice $u=1$ is the [trivial representation](../../../../trivial-representation.md); the unique nontrivial choice is the [sign representation](../../../../sign-representation.md):

$$
\boxed{U(e)=U(y)=U(y^2)=1,\qquad U(x)=U(xy)=U(xy^2)=-1.}
$$

Its [group kernel](../../../../kernel-of-a-group-homomorphism.md) is

$$
\boxed{\ker U=\{e,y,y^2\}.}
$$

A [faithful representation](../../../../faithful-representation.md) is injective and has trivial kernel. Here the kernel has three elements, so **$U$ is not faithful**.

Both one-dimensional representations are [irreducible representations](../../../../irreducible-representation.md), and they are inequivalent to each other and to the given two-dimensional one. The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) gives

$$
1^2+1^2+2^2=6=|S_3|.
$$

These exhaust all complex [irreducible representations](../../../../irreducible-representation.md). Their number equals the number of [conjugacy classes](../../../../conjugacy-class.md), so there are **three conjugacy classes**. Explicitly they are

$$
\boxed{\{e\},\qquad\{y,y^2\},\qquad\{x,xy,xy^2\}.}
$$

The last two sets consist of the 3-cycles and transpositions respectively.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
