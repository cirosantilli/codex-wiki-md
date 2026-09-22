<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

Denote the four displayed matrices, from left to right, by $T_1,T_2,T_3,T_4$. An [orthogonal matrix](../../../../../orthogonal-matrix.md) has an orthonormal set of columns, equivalently $T^TT=I$. Direct column [dot products](../../../../../dot-product.md) give $T_j^TT_j=I$ for $j=1,2,4$. The first column of $T_3$ has squared [Euclidean norm](../../../../../euclidean-norm.md) $(1+6+1)/6=4/3$, so **the third matrix is the unique nonorthogonal matrix**.

For $T_1$, the [determinant](../../../../../determinant.md) is $1$. A nonidentity [orthogonal transformation](../../../../../orthogonal-transformation.md) of $\mathbb R^3$ with [determinant](../../../../../determinant.md) $1$ is a rotation: it has a fixed axis and restricts to a plane rotation on its [orthogonal complement](../../../../../orthogonal-complement.md). Consequently **$T_1$ is the rotation**.

For $T_2$, calculation gives

$$
\det T_2=-1,\qquad \det(T_2-I)=-\frac43.
$$

A plane [reflection](../../../../../reflection-mathematics.md) fixes its entire plane, and therefore has [eigenvalue](../../../../../eigenvalue.md) $1$. Since $T_2-I$ is invertible, $T_2$ is not a plane [reflection](../../../../../reflection-mathematics.md). Thus **$T_2$ is the combination of a rotation and a reflection**. More explicitly, $(1,-2,0)^T$ is an [eigenvector](../../../../../eigenvector.md) with [eigenvalue](../../../../../eigenvalue.md) $-1$. On the perpendicular plane, $T_2$ is a rotation with $\cos\phi=2/3$, because $\operatorname{tr}T_2=-1+2\cos\phi=1/3$. This gives a [three-dimensional improper orthogonal transformation](../../../../../three-dimensional-improper-orthogonal-transformation.md).

For $T_4$, set $n=(1,2,2)^T/3$. Then

$$
T_4=I-2nn^T.
$$

This [reflection matrix](../../../../../reflection-matrix.md) reverses the normal $n$ and fixes every vector perpendicular to $n$. Therefore **$T_4$ is reflection in the plane $x+2y+2z=0$**. In particular, $\det T_4=-1$ and $\det(T_4-I)=0$. Finally **$T_3$ represents none of the three listed orthogonal transformations**, since each preserves the [Euclidean norm](../../../../../euclidean-norm.md).

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
