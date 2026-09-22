<h1 id="36c/solution">Solution</h1>

↑ **Parent:** [36C](../36c.md)

Use SI units, $x^a=(ct,\mathbf x)$ and metric signature $(+,-,-,-)$. The [four-current](../../../../../four-current.md) is $j^a=(c\rho,\mathbf j)$. Charge density and current transform together under Lorentz transformations, and the [continuity equation](../../../../../continuity-equation.md) becomes

$$
\boxed{\partial_aj^a=\partial_t\rho+\nabla\cdot\mathbf j=0.}
$$

With the [four-potential](../../../../../electromagnetic-four-potential.md) $A^a=(\varphi/c,\mathbf A)$, the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) $\partial_aA^a=0$ converts [Maxwell equations](../../../../../maxwell-equations.md) to $\Box A^a=\mu_0j^a$, where $\Box=c^{-2}\partial_t^2-\nabla^2$. Choosing no incoming homogeneous radiation, the [retarded electromagnetic potential](../../../../../retarded-potential.md) is

$$
\boxed{A^a(\mathbf x,t)=\frac{\mu_0}{4\pi}\int\frac{j^a(\mathbf x',t-|\mathbf x-\mathbf x'|/c)}{|\mathbf x-\mathbf x'|}\,d^3x'.}
$$

Current conservation ensures this solution obeys the Lorenz gauge; a homogeneous solution may be added when additional field boundary data are specified.

For a thin loop, let $R=|\mathbf x|$, $\widehat{\mathbf R}=\mathbf x/R$ and $t_R=t-R/c$. Then

$$
\mathbf A=\frac{\mu_0}{4\pi}\oint\frac{I(t-|\mathbf x-\mathbf x'|/c)}{|\mathbf x-\mathbf x'|}\,d\boldsymbol\ell'.
$$

In the small-loop magnetic-dipole approximation, expand $|\mathbf x-\mathbf x'|=R-\widehat{\mathbf R}\cdot\mathbf x'+\cdots$. The constant term integrates to zero because $\oint d\boldsymbol\ell'=0$. The first nonzero term is

$$
\frac{\mu_0}{4\pi}\left[\frac{I(t_R)}{R^2}+\frac{\dot I(t_R)}{cR}\right]\oint(\widehat{\mathbf R}\cdot\mathbf x')\,d\boldsymbol\ell'.
$$

For the oriented circular loop the last integral is $\pi r^2\mathbf n\times\widehat{\mathbf R}$. Thus with [magnetic dipole moment](../../../../../magnetic-dipole-moment.md) $\mathbf m(t)=\pi r^2I(t)\mathbf n$,

$$
\boxed{\mathbf A(\mathbf x,t)=\frac{\mu_0I_0r^2}{4}\left[\frac{\sin(\omega t_R)}{R^2}+\frac{\omega\cos(\omega t_R)}{cR}\right]\mathbf n\times\widehat{\mathbf R}.}
$$

The $R^{-2}$ term is the near dipole potential and the $R^{-1}$ term its radiation potential. This is the leading small-$r$ result at fixed $R,\omega$; besides $r/R\ll1$, the expansion of the retarded current requires $\omega r/c\ll1$.

If only $r/R\ll1$ is imposed and the loop need not be small compared with a wavelength, keep the retarded phase around the loop. For fixed $r,\omega$ and $R\to\infty$, the leading far-field expression is instead

$$
\mathbf A=\frac{\mu_0I_0r}{2R}J_1\left(\frac{\omega r}{c}\sin\theta\right)\cos(\omega t_R)\frac{\mathbf n\times\widehat{\mathbf R}}{\sin\theta}+O(R^{-2}),
$$

where $\cos\theta=\mathbf n\cdot\widehat{\mathbf R}$ and $J_1$ is the [Bessel function of the first kind](../../../../../bessel-function-of-the-first-kind.md). Integrating the sinusoidal phase on a circle gives this Bessel factor; $J_1(z)\sim z/2$ recovers the radiation part of the boxed dipole result.

## ↑ Ancestors (10)

1. [36C](../36c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
