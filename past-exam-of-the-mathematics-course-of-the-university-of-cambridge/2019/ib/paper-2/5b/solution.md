<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

For an axisymmetric separated solution of the [Laplace equation](../../../../../laplace-equation.md) whose angular factor is the [Legendre polynomial](../../../../../legendre-polynomial.md) $P_n(\cos\theta)$, the radial [ordinary differential equation](../../../../../ordinary-differential-equation.md) has the two powers $r^n$ and $r^{-n-1}$. Thus

$$
\boxed{\Phi(r,\theta,\phi)=(A r^n+B r^{-n-1})P_n(\cos\theta)}
$$

for constants $A,B$.

Write $x=\cos\theta$. Since $3\cos(2\theta)=6x^2-3=4P_2(x)-P_0(x)$, only the [spherical harmonics](../../../../../spherical-harmonic.md) of degrees zero and two occur. The degree-zero radial coefficient satisfying its two [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) is $1-2/r$. For degree two, write $Cr^2+Dr^{-3}$; then

$$
C+D=4,
\qquad 4C+\frac D8=0,
$$

so $C=-4/31$ and $D=128/31$. By linearity and uniqueness of this [boundary value problem](../../../../../boundary-value-problem.md),

$$
\boxed{\Phi(r,\theta)=1-\frac2r+
\frac4{31}\left(\frac{32}{r^3}-r^2\right)P_2(\cos\theta)}.
$$

Direct substitution at $r=1,2$ verifies both boundary values.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
