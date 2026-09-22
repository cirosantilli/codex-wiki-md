<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [vector triple product](../../../../vector-triple-product.md) with $|u|=1$ gives

$$
f(r)=r-u(u\cdot r),\qquad\boxed{A=I-uu^T,\quad A_{ij}=\delta_{ij}-u_iu_j.}
$$

This is the [orthogonal projection onto a plane](../../../../closest-point-on-a-plane.md) perpendicular to $u$, so it is a [linear map](../../../../linear-map.md). Its [image](../../../../image-of-a-function.md) is the plane $u^\perp$ through the origin, while its [kernel](../../../../kernel-of-a-linear-map-split.md) is the normal line $\operatorname{span}\{u\}$. In components,

$$
A=\begin{pmatrix}1-u_1^2&-u_1u_2&-u_1u_3\\-u_1u_2&1-u_2^2&-u_2u_3\\-u_1u_3&-u_2u_3&1-u_3^2\end{pmatrix}.
$$

The equation $Ar=r$ is equivalent to $u(u\cdot r)=0$, hence to $u\cdot r=0$. Its solution set is precisely the two-dimensional plane $u^\perp$, with infinitely many nonzero vectors, not merely the normal line. These are the [eigenvectors](../../../../eigenvector.md) with [eigenvalue](../../../../eigenvalue.md) one; the normal direction has [eigenvalue](../../../../eigenvalue.md) zero.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
