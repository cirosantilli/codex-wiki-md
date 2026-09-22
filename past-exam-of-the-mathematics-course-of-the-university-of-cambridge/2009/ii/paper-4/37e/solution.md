<h1 id="37e/solution">Solution</h1>

↑ **Parent:** [37E](../37e.md)

Write the common density as $\rho$ and take positive bending stiffness $\beta$. With $q=|k|>0$, use decaying [velocity potentials](../../../../../velocity-potential.md)

$$
\phi_+=A_+e^{-qy}e^{ikx+\sigma t},\qquad\phi_-=A_-e^{qy}e^{ikx+\sigma t},
$$

added to the upper base potential $Ux$ and the lower zero base potential. They solve the [Laplace equation](../../../../../laplace-equation.md), as required by incompressibility and irrotational flow. The two linear [kinematic boundary conditions](../../../../../kinematic-boundary-condition.md) on the membrane are

$$
-qA_+=(\sigma+ikU)C,\qquad qA_-=\sigma C.
$$

The linearized [Bernoulli equation](../../../../../bernoulli-equation.md) gives perturbation pressures $p'_+=-\rho(\sigma+ikU)A_+$ and $p'_-=-\rho\sigma A_-$. Substituting the kinematic conditions and imposing the stipulated pressure difference gives

$$
p'_- -p'_+=-\frac\rho q[\sigma^2+(\sigma+ikU)^2]C=\beta k^4C.
$$

Completing the square yields the [bending-membrane Kelvin-Helmholtz dispersion relation](../../../../../bending-membrane-kelvin-helmholtz-dispersion-relation.md)

$$
\boxed{\left(\sigma+\frac{ikU}{2}\right)^2=\frac{U^2k^2}{4}-\frac{\beta|k|^5}{2\rho}.}
$$

The imaginary shift convects the disturbance at mean fluid speed $U/2$. For $U\ne0$ there is a growing root exactly when

$$
\boxed{0<|k|<k_{\max},\qquad k_{\max}=\left(\frac{\rho U^2}{2\beta}\right)^{1/3}.}
$$

At $k=0$ the uniform displacement is neutral; at $|k|=k_{\max}$ the square-root growth vanishes. Above this cutoff both roots are imaginary. To maximize the growth, maximize its square $U^2q^2/4-\beta q^5/(2\rho)$ over the unstable interval. Its derivative is $U^2q/2-5\beta q^4/(2\rho)$, so its unique positive maximum is

$$
\boxed{q_* =\left(\frac{\rho U^2}{5\beta}\right)^{1/3}=\left(\frac25\right)^{1/3}k_{\max},\qquad
\operatorname{Re}\sigma_{\max}=|U|q_*\sqrt{\frac3{20}}.}
$$

For $U=0$ there is no [Kelvin-Helmholtz instability](../../../../../kelvin-helmholtz-instability.md). Positivity of $\beta$ is the physical stiffness assumption behind the finite cutoff: $\beta=0$ gives no upper unstable cutoff, and $\beta<0$ destabilizes arbitrarily short waves.

## ↑ Ancestors (10)

1. [37E](../37e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
