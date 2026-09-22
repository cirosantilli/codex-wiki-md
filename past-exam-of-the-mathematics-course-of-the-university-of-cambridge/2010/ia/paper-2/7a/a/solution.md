<h1 id="7a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the coefficient matrix as $M$. Its [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $\det(rI-M)=r(r-2)(r+2)$. Corresponding [eigenvectors](../../../../../../eigenvector.md) are

$$
v_-=(-1,1,1)^T,\qquad v_0=(1,1,1)^T,\qquad
v_+=(-1,-1,1)^T,
$$

with [eigenvalues](../../../../../../eigenvalue.md) $-2,0,2$ respectively, as direct multiplication verifies. Distinct [eigenvalues](../../../../../../eigenvalue.md) make these vectors a basis. Expanding a solution as $z_-v_-+z_0v_0+z_+v_+$ decouples the [linear ordinary differential equations](../../../../../../linear-ordinary-differential-equation.md) into $\dot z_-=-2z_-$, $\dot z_0=0$, $\dot z_+=2z_+$. Thus **the general solution is**

$$
\boxed{\begin{pmatrix}x\\y\\z\end{pmatrix}
=Ae^{-2t}v_-+Bv_0+Ce^{2t}v_+.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7A](../../7a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
