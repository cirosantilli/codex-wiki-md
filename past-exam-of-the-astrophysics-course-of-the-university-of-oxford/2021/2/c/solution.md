<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First retain the exact initial normalization. The [scale factor](../../../../scale-factor-cosmology.md) obeys $a/a_i=(t/t_i)^{2/3}$, so the [cosmological redshift](../../../../cosmological-redshift.md) is

$$
1+z=(1+z_i)\left[\frac{t_i}{B(\theta-\sin\theta)-T}\right]^{2/3}.
$$

Also $\rho=3M/(4\pi r^3)$ and $\rho_m=1/(6\pi Gt^2)$. Using $A^3=GMB^2$ gives

$$
1+\delta=\frac92\frac{[\theta-\sin\theta-T/B]^2}{(1-\cos\theta)^3}.
$$

These equations exactly accommodate the finite-time initial conditions in [b](../b.md).

Now neglect $T$ and retain leading order in $\delta_i\ll1$. Since $t_i/B=4\delta_i^{3/2}/[3(1+\delta_i)]$, the [cosmological redshift](../../../../cosmological-redshift.md) relation reduces to

$$
1+z\simeq\left(\frac43\right)^{2/3}\frac{\delta_i(1+z_i)}{(\theta-\sin\theta)^{2/3}}.
$$

Define $\delta_0=\frac35\delta_i(1+z_i)$. Then

$$
\boxed{1+z\simeq\frac53\left(\frac43\right)^{2/3}
\frac{\delta_0}{(\theta-\sin\theta)^{2/3}},\qquad
\delta\simeq\frac92\frac{(\theta-\sin\theta)^2}{(1-\cos\theta)^3}-1.}
$$

The second equality is exact for the ideal common-bang growing-mode [spherical-collapse model](../../../../spherical-collapse-model.md); it is approximate for the paper's finite-time initial Hubble-velocity data.

The factor $3/5$ has a physical origin. Linear mass conservation gives $\dot\delta_i=0$ when the initial local expansion equals the background [Hubble flow](../../../../hubble-flow.md). The general linear dust solution is $\delta_L=C_g(t/t_i)^{2/3}+C_d(t/t_i)^{-1}$. Imposing $\delta_L(t_i)=\delta_i$ and $\dot\delta_L(t_i)=0$ yields

$$
\delta_L(t)=\frac35\delta_i\left(\frac t{t_i}\right)^{2/3}
+\frac25\delta_i\left(\frac t{t_i}\right)^{-1}.
$$

Thus $\delta_0$ is the present extrapolation of the _growing component_, after neglecting the decaying transient. It is not the exact present value of the full linear solution for finite $t_i$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
