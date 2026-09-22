<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Vary $r$ by $r+\varepsilon\eta$ with $\eta(a)=\eta(b)=0$. The first [variation](../../../../variation.md) of the [functional](../../../../functional.md) is

$$
\delta I_1=\int_a^b(F_{1,r}\eta+F_{1,r'}\eta')dz=\int_a^b\left(F_{1,r}-\frac d{dz}F_{1,r'}\right)\eta\,dz.
$$

The boundary term from [integration by parts](../../../../integration-by-parts.md) is zero. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives $\boxed{F_{1,r}-dF_{1,r'}/dz=0}$. For $I_2$, independently vary $r$ and $\theta$ with zero endpoint variations; the two [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
\boxed{F_{2,r}-\frac d{dz}F_{2,r'}=0,\qquad F_{2,\theta}-\frac d{dz}F_{2,\theta'}=0.}
$$

For the optical path, [Fermat principle](../../../../fermat-principle.md) makes $\int\mu\,ds$ stationary. In [cylindrical coordinates](../../../../cylindrical-coordinate-system.md) its [integrand](../../../../integrand.md) is $L=\mu(r,\theta)s$, with $s=\sqrt{1+r'^2+r^2\theta'^2}$. There is no explicit $z$ dependence. The [Beltrami identity for several dependent variables](../../../../beltrami-identity-for-several-dependent-variables.md) gives

$$
L-r'L_{r'}-\theta'L_{\theta'}=\mu s-\frac{\mu(r'^2+r^2\theta'^2)}s=\frac\mu s=\text{constant}.
$$

The conserved quantity is the axial component of the [optical momentum of a ray](../../../../optical-momentum-of-a-ray.md). As $\mu>0$, squaring and inverting yields

$$
\boxed{\frac{1+r'^2+r^2\theta'^2}{\mu^2}=\text{constant}.}
$$

Now suppose $\mu=\mu(r)$ and seek a path of radius $R>0$. The angle is a [cyclic coordinate](../../../../cyclic-coordinate.md), so $L_{\theta'}=\mu R^2\theta'/\sqrt{1+R^2\theta'^2}$ is conserved. At fixed radius this is strictly increasing in $\theta'$, forcing $\theta'=\omega$ constant. The radial [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) reduces to

$$
\mu'(R)(1+R^2\omega^2)+\mu(R)R\omega^2=0.
$$

Consequently the [helical rays in a radially graded refractive index](../../../../helical-rays-in-a-radially-graded-refractive-index.md) have

$$
\boxed{r(z)=R,\qquad\theta(z)=\theta_0+\omega z,\qquad\omega^2=-\frac{\mu'(R)}{R[\mu(R)+R\mu'(R)]}.}
$$

A real nonzero [helix](../../../../helix.md) exists at such a radius when $0<-R\mu'(R)/\mu(R)<1$, and its [helical pitch](../../../../pitch-of-a-helix.md) is $2\pi/|\omega|$. If $\mu'(R)=0$, the solution is instead a straight axial [light ray](../../../../light-ray.md). Thus radial dependence permits constant-radius rays for suitable profiles; an arbitrary radial profile need not support a nonzero real [helix](../../../../helix.md). This qualification is necessary, for example when the [refractive index](../../../../refractive-index.md) increases with radius.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 1](../../paper-1-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
