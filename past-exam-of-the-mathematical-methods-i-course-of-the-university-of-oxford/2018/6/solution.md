<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [characteristic polynomial](../../../characteristic-polynomial.md) factors as $\det(\lambda I-A)=(\lambda-1)(\lambda^2-1)$. Thus $\boxed{\lambda=1\text{ twice},\quad\lambda=-1\text{ once}}$ in [algebraic multiplicity](../../../algebraic-multiplicity.md). An [orthonormal basis](../../../orthonormal-basis.md) of corresponding [eigenvectors](../../../eigenvector.md) is

$$
v_1=\begin{pmatrix}1\\0\\0\end{pmatrix},\quad
v_2=\frac1{\sqrt2}\begin{pmatrix}0\\1\\-i\end{pmatrix}\quad(\lambda=1),\qquad
v_3=\frac1{\sqrt2}\begin{pmatrix}0\\1\\i\end{pmatrix}\quad(\lambda=-1).
$$

Direct multiplication verifies $Av_1=v_1$, $Av_2=v_2$, $Av_3=-v_3$. Their mutual [Hermitian inner products](../../../hermitian-inner-product.md) vanish and each has [norm](../../../norm.md) one, which proves [linear independence](../../../linear-independence.md). For the repeated [eigenvalue](../../../eigenvalue.md), [Gaussian elimination](../../../gaussian-elimination.md) gives

$$
A-I=\begin{pmatrix}0&0&0\\0&-1&i\\0&-i&-1\end{pmatrix}
\ \longrightarrow\ 
\begin{pmatrix}0&1&-i\\0&0&0\\0&0&0\end{pmatrix}.
$$

Hence $\boxed{\operatorname{rank}(A-I)=1,\quad\dim\ker(A-I)=2}$. The second equality follows from the [rank-nullity theorem](../../../rank-nullity-theorem.md) and agrees with the two-dimensional [eigenspace](../../../eigenspace.md). A repeated [eigenvalue](../../../eigenvalue.md) alone would not imply a two-dimensional [eigenspace](../../../eigenspace.md) for an arbitrary [matrix](../../../matrix.md); here the [Hermitian matrix](../../../hermitian-operator.md) is [diagonalizable](../../../diagonalizable-matrix.md).

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2018](../../2018-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
