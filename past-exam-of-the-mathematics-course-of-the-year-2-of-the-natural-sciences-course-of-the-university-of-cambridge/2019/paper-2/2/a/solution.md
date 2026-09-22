<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a separated [axisymmetric harmonic function](../../../../../axisymmetric-harmonic-function.md) $\Psi=R(r)\Theta(\theta)$, multiplying the [Laplace equation](../../../../../laplace-equation.md) by $r^2/(R\Theta)$ gives

$$
\frac{(r^2R')'}{R}
=-\frac{(\sin\theta\,\Theta')'}{\sin\theta\,\Theta}=\lambda.
$$

The two sides depend on different variables, hence both equal a constant. Put $u=\cos\theta$ in the angular equation. Since $\sin\theta\,\Theta'=-\sin^2\theta\,d\Theta/du$, it becomes the [Legendre differential equation](../../../../../legendre-differential-equation.md)

$$
\frac{d}{du}\left[(1-u^2)\frac{d\Theta}{du}\right]+\lambda\Theta=0.
$$

Regularity on both parts of the polar axis restricts $\lambda=\ell(\ell+1)$, with $\ell=0,1,\ldots$, and selects the [Legendre polynomial](../../../../../legendre-polynomial.md) $P_\ell(u)$. The other angular solution is singular at an endpoint.

The radial [Euler differential equation](../../../../../cauchy-euler-equation.md) is

$$
r^2R''+2rR'-\ell(\ell+1)R=0.
$$

Trying $R=r^s$ gives $s(s+1)=\ell(\ell+1)$, so $s=\ell$ or $s=-\ell-1$. [Superposition](../../../../../superposition-principle.md) of these separated [harmonic functions](../../../../../harmonic-function.md) gives

$$
\boxed{\Psi(r,\theta)=\sum_{\ell=0}^\infty
\left(A_\ell r^\ell+B_\ell r^{-\ell-1}\right)P_\ell(\cos\theta)}.
$$

The [Legendre polynomials](../../../../../legendre-polynomial.md) form the angular expansion for regular data with [rotational symmetry](../../../../../rotational-symmetry.md) about the polar axis; the radial domain and the [boundary conditions](../../../../../boundary-condition.md) determine which coefficients survive and where the expansion converges.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
