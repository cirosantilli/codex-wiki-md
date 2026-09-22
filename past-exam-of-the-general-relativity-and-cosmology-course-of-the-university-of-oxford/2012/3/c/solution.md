<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A radial null ray satisfies $dr/\sqrt{1-kr^2}=\pm c\,dt/a(t)$. Define the present-normalized radial [comoving distance](../../../../comoving-radial-distance.md)

$$
D_C=\int_{t_E}^{t_0}\frac{c\,dt}{a(t)}=\int_0^{r_E}\frac{dr}{\sqrt{1-kr^2}}.
$$

For $k<0$, write $\kappa=\sqrt{-k}=H_0\sqrt{\Omega_K}/c$. Integration gives $D_C=\operatorname{arsinh}(\kappa r_E)/\kappa$, so $r_E=\sinh(\kappa D_C)/\kappa$. Two neighboring pulses on the same comoving path obey $\Delta t_0/a_0=\Delta t_E/a_E$, hence $1+z=1/a_E$. For the [angular diameter distance in an open dust universe](../../../../angular-diameter-distance-in-an-open-dust-universe.md), a transverse source size $\ell=a_Er_E\,\delta\theta$ defines the [angular diameter distance](../../../../angular-diameter-distance.md) $D_A=\ell/\delta\theta$. Thus

$$
\boxed{D_A(z)=\frac1{1+z}\frac{c}{H_0\sqrt{\Omega_K}}\sinh\left(\frac{H_0\sqrt{\Omega_K}}cD_C(z)\right).}
$$

Since $dt=da/(aH)$, the dust-plus-curvature expansion gives

$$
\boxed{D_C(z)=\frac c{H_0}\int_{1/(1+z)}^1\frac{da}{\sqrt a\sqrt{\Omega_M+(1-\Omega_M)a}}.}
$$

At a specified source redshift, the only independent cosmological parameters in this integral are $\Omega_M$ and $H_0$. The distance necessarily also has a source-position argument; it cannot be a constant for all sources.

For $0<\Omega_M<1$, the integral can be written

$$
D_C=\frac{2c}{H_0\sqrt{1-\Omega_M}}\left[\operatorname{arsinh}\sqrt{\frac{1-\Omega_M}{\Omega_M}}-\operatorname{arsinh}\sqrt{\frac{1-\Omega_M}{\Omega_M(1+z)}}\right].
$$

The apparently singular parameter endpoints have regular limits: $\Omega_M=0$ gives $D_C=(c/H_0)\ln(1+z)$, and $\Omega_M=1$ gives $D_C=(2c/H_0)[1-(1+z)^{-1/2}]$. The flat-curvature distance limit is $D_A=D_C/(1+z)$. For a negative $\Omega_K$, the transverse distance uses sine with $\sqrt{-\Omega_K}$ instead of hyperbolic sine; that closed case is outside the almost-empty open model, but explains the convention behind the square root.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
