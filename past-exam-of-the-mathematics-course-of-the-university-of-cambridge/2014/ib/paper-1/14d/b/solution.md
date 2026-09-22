<h1 id="14d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $U=R(r)\Theta(\theta)$ in the [Laplace equation](../../../../../../laplace-equation.md), multiply by $r^2/U$, and separate:

$$
\frac1R(r^2R')'=\lambda,\qquad \frac1{\sin\theta}(\sin\theta\Theta')'+\lambda\Theta=0.
$$

Putting $x=\cos\theta$ turns the angular equation into the [Legendre differential equation](../../../../../../legendre-differential-equation.md). For a solution smooth on the whole spherical axis, the allowed eigenvalues are $\lambda=n(n+1)$ with angular functions $P_n(\cos\theta)$. The radial equation has the two solutions $r^n,r^{-n-1}$. Superposition yields the regular axisymmetric expansion

$$
\boxed{U(r,\theta)=\sum_{n=0}^\infty(A_nr^n+B_nr^{-n-1})P_n(\cos\theta).}
$$

The coefficients and convergence region are set by the domain and boundary data. Without regularity at the poles, singular Legendre functions and more general separated degrees would also be possible; they are excluded for this exterior spherical field.

The far-field matching fixes $A_1=v_0$ and all other growing coefficients to zero. The radial [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) at $r_0$ is

$$
\sum_{n=0}^\infty[nA_nr_0^{n-1}-(n+1)B_nr_0^{-n-2}]P_n(\cos\theta)=0.
$$

Independence of the angular modes gives $B_1=v_0r_0^3/2$ and all other decaying coefficients zero. Thus the [exterior harmonic potential with no flux through a sphere](../../../../../../exterior-harmonic-potential-with-no-flux-through-a-sphere.md) is

$$
\boxed{U=v_0\left(r+\frac{r_0^3}{2r^2}\right)\cos\theta.}
$$

Its derivative vanishes on the sphere and its difference from $v_0r\cos\theta$ tends to zero at infinity. A spatial constant may be added if the far-field condition is intended only to specify the gradient or the leading growing term; matching the potential difference to zero fixes that constant to zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14D](../../14d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
