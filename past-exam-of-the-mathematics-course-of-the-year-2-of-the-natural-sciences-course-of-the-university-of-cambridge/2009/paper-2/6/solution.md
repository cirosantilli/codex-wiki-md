<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An [isotropic tensor](../../../../isotropic-tensor.md) has unchanged components under every proper rotation of the Cartesian axes. Every rank-zero [scalar](../../../../scalar.md) is isotropic, and $c\delta_{ij}$ is a rank-two example. The zero rank-one tensor is isotropic, but no nonzero [vector](../../../../vector.md) is: a half-turn about an axis perpendicular to it reverses its sign.

For the [inertia tensor](../../../../inertia-tensor.md), write $u=x-G$ and $X=P-G$, so $x-P=u-X$. Expand its defining integrand. Every cross term has an integral containing $\int_Bu\rho\,d^3x=0$ by the definition of the [centre of mass](../../../../center-of-mass.md). The remaining terms give the [tensor parallel-axis theorem](../../../../tensor-parallel-axis-theorem.md):

$$
\boxed{I_{ij}(P)-I_{ij}(G)=M(|X|^2\delta_{ij}-X_iX_j).}
$$

For a uniform unit ball, rotational symmetry gives $\int\rho u_iu_jd^3u=c\delta_{ij}$. Its trace is $\int\rho|u|^2d^3u=3M/5$, so $c=M/5$ and $I(G)=2MI/5$. Therefore

$$
\boxed{I(P)=M\left[\left(\frac25+|X|^2\right)I-XX^T\right].}
$$

Assuming positive mass, it is isotropic exactly when **$P=G$**. For $X\ne0$, its [eigenvalues](../../../../eigenvalue.md) and directions are

$$
\boxed{\lambda_\parallel=\frac{2M}{5},\quad e_\parallel=X/|X|;\qquad
\lambda_\perp=M\left(\frac25+|X|^2\right)\quad\text{on }X^\perp.}
$$

To give an explicit orthonormal [eigenbasis](../../../../eigenbasis.md) when $X_1^2+X_2^2>0$, take $e_1=(-X_2,X_1,0)/\sqrt{X_1^2+X_2^2}$ and $e_2=e_\parallel\times e_1$. If $X$ is a nonzero [vector](../../../../vector.md) along the third axis, take the first two coordinate [unit vectors](../../../../unit-vector.md) instead. At $X=0$, all three [eigenvalues](../../../../eigenvalue.md) are $2M/5$ and every [orthonormal basis](../../../../orthonormal-basis.md) works. The [inertia tensor of a displaced uniform ball](../../../../inertia-tensor-of-a-displaced-uniform-ball.md) describes the same result for an arbitrary radius.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
