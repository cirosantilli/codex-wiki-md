<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

A [group homomorphism](../../../../group-homomorphism.md) is a multiplication-preserving map $\phi:G_1\to G_2$, so $\phi(gh)=\phi(g)\phi(h)$. A [group isomorphism](../../../../group-isomorphism.md) is a bijective homomorphism; its inverse is automatically multiplication-preserving as well.

For the real [general linear group](../../../../general-linear-group.md), the identity matrix has nonzero determinant. If $A,B$ have nonzero determinants, [multiplicativity of the determinant](../../../../multiplicativity-of-the-determinant.md) gives $\det(AB)=\det A\det B\ne0$. Associativity is inherited from matrix multiplication, and every such matrix has an inverse, with $\det A^{-1}=1/\det A\ne0$. Hence the given set $\operatorname{GL}(n,\mathbb R)$ is a group.

For the [special orthogonal group](../../../../special-orthogonal-group.md), the identity is included and

$$
(AB)(AB)^T=A(BB^T)A^T=I,\qquad\det(AB)=1
$$

when both factors are special orthogonal. Moreover $A^{-1}=A^T$ is again orthogonal and has determinant one. Thus $\operatorname{SO}(n)$ is a subgroup. The [orientation-preserving general linear group](../../../../orientation-preserving-general-linear-group.md) is also a subgroup: the identity has positive determinant, products preserve positivity, and inversion replaces the determinant by its positive reciprocal.

Now take an element $\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$ of the [special orthogonal group in two dimensions](../../../../special-orthogonal-group-in-two-dimensions.md). Orthogonality and determinant one imply

$$
\begin{pmatrix}a&c\\b&d\end{pmatrix}=A^T=A^{-1}=\begin{pmatrix}d&-b\\-c&a\end{pmatrix}.
$$

Hence $d=a$, $b=-c$, and the unit length of the first column gives $a^2+c^2=1$. There is an angle $\theta$, unique modulo $2\pi$, such that $a=\cos\theta$, $c=\sin\theta$. Therefore

$$
\boxed{A=R(\theta)=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}.}
$$

Define the map from the [circle group](../../../../circle-group.md) by

$$
\boxed{\phi:U(1)\longrightarrow\operatorname{SO}(2),\qquad a+ic\longmapsto\begin{pmatrix}a&-c\\c&a\end{pmatrix}.}
$$

If $z=a+ic$ and $w=p+iq$, matrix multiplication gives $\phi(z)\phi(w)=\left(\begin{smallmatrix}ap-cq&-(aq+cp)\\aq+cp&ap-cq\end{smallmatrix}\right)=\phi(zw)$. Thus it is a homomorphism. The entries determine $a,c$ uniquely, proving injectivity, and the parametrization proves surjectivity. This establishes

$$
\boxed{\operatorname{SO}(2)\cong U(1).}
$$

The use of the unit complex number, rather than an unrestricted real angle, removes the $2\pi$ ambiguity: angles add modulo $2\pi$, exactly as unit complex numbers multiply.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 2](../../paper-2-split.md)
3. [2012](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
