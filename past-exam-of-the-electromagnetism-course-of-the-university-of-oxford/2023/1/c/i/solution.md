<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $r_0=|\mathbf r_0|$ and let $\Omega_0=(\theta_0,\varphi_0)$ describe its direction in [spherical coordinates](../../../../../spherical-coordinate-system.md); write $\Omega=(\theta,\varphi)$. The given [Dirichlet Green function between concentric spheres](../../../../../dirichlet-green-function-between-concentric-spheres.md) has normalization $\nabla^2G=-4\pi\delta^{(3)}$, so the [electric potential](../../../../../electric-potential.md) is $\phi=qG/(4\pi\epsilon_0)$. On the inner sphere the [unit normal](../../../../../unit-normal.md) from metal into the gap is $+\mathbf e_r$, hence its induced [surface charge density](../../../../../surface-charge-density.md) is

$$
\sigma(a,\Omega)=-\frac q{4\pi}\left.\partial_rG(r,\Omega;\mathbf r_0)\right|_{a^+}.
$$

Near this boundary $r_<=r$ and $r_>=r_0$. The needed radial [derivative](../../../../../derivative.md) is

$$
\left.\frac{d}{dr}\left(r^\ell-\frac{a^{2\ell+1}}{r^{\ell+1}}\right)\right|_{r=a}
=\ell a^{\ell-1}+(\ell+1)a^{\ell-1}=(2\ell+1)a^{\ell-1}.
$$

It cancels the factor $2\ell+1$ in the [Dirichlet Green function](../../../../../dirichlet-green-function.md). Therefore the answer in [spherical harmonics](../../../../../spherical-harmonic.md) is

$$
\boxed{\sigma(a,\Omega)=-q\sum_{\ell=0}^{\infty}\sum_{m=-\ell}^{\ell}
\frac{a^{\ell-1}\overline{Y_{\ell m}(\Omega)}Y_{\ell m}(\Omega_0)}{1-(a/b)^{2\ell+1}}
\left(\frac1{r_0^{\ell+1}}-\frac{r_0^\ell}{b^{2\ell+1}}\right).}
$$

This [spherical harmonic](../../../../../spherical-harmonic.md) expansion converges on the boundary: after the angular sum, the two radial factors decay geometrically with ratios $a/r_0<1$ and $ar_0/b^2<1$, while the angular factors grow at most polynomially. This justifies the boundary [derivative](../../../../../derivative.md) and the subsequent [surface integral](../../../../../surface-integral.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
