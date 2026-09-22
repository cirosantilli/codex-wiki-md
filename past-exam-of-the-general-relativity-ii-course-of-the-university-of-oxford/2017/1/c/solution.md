<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [geodesic deviation](../../../../geodesic-deviation.md) equation compares neighboring [geodesics](../../../../geodesic.md) by [covariant derivatives](../../../../covariant-derivative.md). Replacing those derivatives by ordinary derivatives of coordinate components requires a [parallel transport](../../../../parallel-transport.md) frame along the reference [geodesic](../../../../geodesic.md). There is also an [affine parameter](../../../../affine-parameter.md) normalization to specify: the argument of $M$ is $u$, and it becomes $\tau$ only after choosing $u=\tau$.

For the intended local tidal calculation, take the reference [timelike geodesic](../../../../timelike-geodesic.md)

$$
\gamma(\tau)=(u,v,x,y)=(\tau,-\tau/2,0,0),
\qquad
V=\partial_u-\frac12\partial_v.
$$

Here $g(V,V)=-1$, so $\tau$ is [proper time](../../../../proper-time.md). Both $F$ and its first [partial derivatives](../../../../partial-derivative.md) vanish on $\gamma$. All [Christoffel symbols](../../../../christoffel-symbol.md) therefore vanish along this curve, and its [coordinate basis](../../../../coordinate-basis.md) is [parallel transport](../../../../parallel-transport.md) along it. With the [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) from part (b),

$$
R^i{}_{uju}=-M_{ij},\qquad
R^u{}_{bcd}=0,\qquad
R^v{}_{uju}=0\quad\text{on }\gamma.
$$

The [Jacobi field](../../../../jacobi-field.md) equation thus becomes, in this adapted frame,

$$
\boxed{
\ddot\sigma^u=0,\qquad
\ddot\sigma^v=0,\qquad
\ddot\sigma^i=M_{ij}(\tau)\sigma^j.
}
$$

A purely transverse initial [Jacobi field](../../../../jacobi-field.md), with $\sigma^u=\sigma^v=\dot\sigma^u=\dot\sigma^v=0$ initially, remains transverse. This [transverse tidal equation of a Brinkmann plane wave](../../../../transverse-tidal-equation-of-a-brinkmann-plane-wave.md) describes the relative [tidal acceleration](../../../../tidal-acceleration.md) of the freely falling bodies.

In vacuum write the [symmetric matrix](../../../../symmetric-matrix.md) as

$$
M(u)=
\begin{pmatrix}
A(u)&B(u)\\ B(u)&-A(u)
\end{pmatrix}.
$$

Its instantaneous [eigenvalues](../../../../eigenvalue.md) are $\pm\sqrt{A^2+B^2}$. The [tidal acceleration](../../../../tidal-acceleration.md) stretches along one principal axis and squeezes along the perpendicular axis, with the axes allowed to vary with $u$. This describes accelerations; it does not imply monotonically growing and shrinking separations for arbitrary initial velocities. For the simple constant profile $A=\omega^2$, $B=0$,

$$
\sigma^x=C\cosh(\omega\tau)+D\sinh(\omega\tau),
\qquad
\sigma^y=P\cos(\omega\tau)+Q\sin(\omega\tau).
$$

Thus the [geodesic deviation](../../../../geodesic-deviation.md) can be defocusing in one direction and oscillatory in the other. For a varying profile, diagonalizing at each instant does not decouple the [ordinary differential equations](../../../../ordinary-differential-equation.md) without also including derivatives of the rotating [eigenvectors](../../../../eigenvector.md).

**Qualification of the coordinate claim.** The displayed equation for $\sigma^v$ is not true for arbitrary coordinate displacements along arbitrary reference [geodesics](../../../../geodesic.md). For synchronized neighboring curves with $u=\tau$ and $\sigma^u=0$, the exact [geodesic equations](../../../../geodesic-equation.md) are

$$
\ddot{\mathbf x}=M\mathbf x,\qquad
\ddot v=-\frac12\mathbf x^{T}M'\mathbf x
-2\dot{\mathbf x}^{T}M\mathbf x.
$$

Their variation gives

$$
\ddot{\boldsymbol\sigma}_{\perp}=M\boldsymbol\sigma_{\perp},\qquad
\ddot\sigma^v
=-\mathbf x^{T}M'\boldsymbol\sigma_{\perp}
-2\dot{\mathbf x}^{T}M\boldsymbol\sigma_{\perp}
-2\mathbf x^{T}M\dot{\boldsymbol\sigma}_{\perp}.
$$

The second expression need not vanish. A concrete vacuum counterexample is $M=\operatorname{diag}(1,-1)$ and the one-parameter family of [timelike geodesics](../../../../timelike-geodesic.md)

$$
u=\tau,\qquad
x=Ae^\tau,\qquad
y=0,\qquad
v=-\frac{\tau}{2}-\frac{A^2}{2}e^{2\tau}.
$$

Each has $g(V,V)=-1$. Differentiating with respect to $A$ produces a [Jacobi field](../../../../jacobi-field.md)

$$
\sigma^u=0,\qquad
\sigma^x=e^\tau,\qquad
\sigma^y=0,\qquad
\sigma^v=-Ae^{2\tau},
\qquad
\ddot\sigma^v=-4Ae^{2\tau}.
$$

This even has $g(V,\sigma)=0$, so it is a physical orthogonal separation. The [covariant derivative](../../../../covariant-derivative.md) form of [geodesic deviation](../../../../geodesic-deviation.md) remains correct; the unrestricted assertion about ordinary coordinate derivatives needs the adapted reference and frame used above. If instead $\dot u=c$ is a constant [affine parameter](../../../../affine-parameter.md) normalization, the transverse tidal coefficient is $c^2M(u)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
