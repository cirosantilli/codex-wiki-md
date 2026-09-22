<h1 id="12/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a real orthonormal [basis](../../../../basis.md), a [matrix](../../../../matrix.md) is a proper [rotation matrix](../../../../rotation-matrix.md) exactly when $R^TR=I$ and $\det R=1$. The first condition preserves [dot products](../../../../dot-product.md), and the second preserves [orientation of a vector space](../../../../orientation-of-a-vector-space.md).

Put $s=\sqrt3$, $p=(1+s)/3$, $q=(1-s)/3$ and $r=1/3$, so the rows of the given [matrix](../../../../matrix.md) are $(p,q,r),(r,p,q),(q,r,p)$. Their squared [Euclidean norms](../../../../euclidean-norm.md) and pairwise [dot products](../../../../dot-product.md) are

$$
p^2+q^2+r^2=1,\qquad pq+qr+rp=0.
$$

Thus $R^TR=I$. For the sign of its [determinant](../../../../determinant.md), use the circulant form:

$$
\det R=p^3+q^3+r^3-3pqr
=(p+q+r)(p^2+q^2+r^2-pq-qr-rp)=1.
$$

This proves that it is a [rotation matrix](../../../../rotation-matrix.md). Its fixed axis is $(1,1,1)^T$, because each row sums to one. The [rotation trace formula](../../../../trace-of-a-three-dimensional-rotation.md) gives $\cos\theta=(\operatorname{tr}R-1)/2=\sqrt3/2$; the skew part selects a positive [angle](../../../../angle.md) $\theta=\pi/6$ about the unit axis $(1,1,1)^T/\sqrt3$.

The original triangle has edge [vectors](../../../../vector.md) $b-a=(-2,2,0)^T$ and $c-a=(-2,0,2)^T$. Its [area](../../../../surface-area.md) is half the [Euclidean norm](../../../../euclidean-norm.md) of their [cross product](../../../../cross-product.md):

$$
\boxed{\mathcal A=\tfrac12\|(b-a)\times(c-a)\|=\tfrac12\|(4,4,4)^T\|=2\sqrt3.}
$$

The rotated vertices are twice the three columns of $R$:

$$
\boxed{a'=\frac23\begin{pmatrix}1+\sqrt3\\1\\1-\sqrt3\end{pmatrix},\qquad
b'=\frac23\begin{pmatrix}1-\sqrt3\\1+\sqrt3\\1\end{pmatrix},\qquad
c'=\frac23\begin{pmatrix}1\\1-\sqrt3\\1+\sqrt3\end{pmatrix}.}
$$

A [rotation matrix](../../../../rotation-matrix.md) preserves lengths and the [angle](../../../../angle.md) between the two edge [vectors](../../../../vector.md), so it preserves their parallelogram [area](../../../../surface-area.md). More explicitly, $(Ru)\times(Rv)=R(u\times v)$ for a proper [rotation matrix](../../../../rotation-matrix.md), and $R(1,1,1)^T=(1,1,1)^T$, so the rotated edge [cross product](../../../../cross-product.md) is again $(4,4,4)^T$. Therefore

$$
\boxed{\mathcal A'=2\sqrt3.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [12](../../12.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
