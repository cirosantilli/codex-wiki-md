<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret the square as $[0,1]^2$, use equal spacing $h=1/J$ in both directions and retain interior indices $1\leq m,n\leq J-1$. Boundary values contribute to the right-hand side and do not change the interior coefficient [matrix](../../../../../../matrix.md). Products of the one-dimensional sine modes used in the [discrete sine transform](../../../../../../discrete-sine-transform.md)

$$
v_{pq}(m,n)=\sin(p\pi m/J)\sin(q\pi n/J)
$$

form a [basis](../../../../../../basis.md), and substitution into the [five-point Laplacian](../../../../../../five-point-laplacian.md) gives

$$
\Delta_hv_{pq}=-\Lambda_{pq}v_{pq},\qquad
\Lambda_{pq}=\frac4{h^2}\left[
\sin^2\left(\frac{p\pi}{2J}\right)+
\sin^2\left(\frac{q\pi}{2J}\right)\right].
$$

The interior [matrix](../../../../../../matrix.md) is $\Delta_h+\lambda I$, so it is nonsingular exactly when

$$
\boxed{\lambda\notin\{\Lambda_{pq}:1\leq p,q\leq J-1\}.}
$$

These are the [discrete Helmholtz resonance](../../../../../../discrete-helmholtz-resonance.md) values, including their possible multiplicities. A sufficient condition is $\lambda<\Lambda_{11}=8h^{-2}\sin^2(\pi/(2J))$, so in particular every nonpositive $\lambda$ is allowed. That is not a necessary restriction: positive values between, or above, the finitely many discrete [eigenvalues](../../../../../../eigenvalue.md) are nonsingular as well. With homogeneous [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) a nonresonant system has only the zero solution; at a resonance the corresponding modes of the [discrete sine transform](../../../../../../discrete-sine-transform.md) give nonzero homogeneous solutions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
