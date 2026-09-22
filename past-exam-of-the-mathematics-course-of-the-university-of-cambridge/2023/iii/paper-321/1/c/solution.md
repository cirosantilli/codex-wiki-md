<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the perturbations as $(\sigma,u,v)e^{ik_xx+\lambda t}$, set $k=|k_x|$, and evaluate all unmarked background quantities at $\Sigma_0$. Define

$$
v_s^2=\left.\frac{dP}{d\Sigma}\right|_{\Sigma_0},
\qquad
\beta=\left.\frac{d\ln(\nu\Sigma)}{d\ln\Sigma}\right|_{\Sigma_0}.
$$

The linearized [mass conservation](../../../../../../mass-conservation.md) equation is

$$
\lambda\sigma+ik_x\Sigma_0u=0.
$$

The radial and azimuthal momentum equations are

$$
\left[\lambda+\left(\nu_b+\frac43\nu\right)k^2\right]u-2\Omega v
=-ik_x\left(v_s^2\frac{\sigma}{\Sigma_0}+\phi\right),
$$



$$
(\lambda+\nu k^2)v+(2\Omega-S)u
=-ik_xS\beta\nu\frac{\sigma}{\Sigma_0},
$$

where the [razor-thin disk Poisson kernel](../../../../../../razor-thin-disk-poisson-kernel.md) gives $\phi=-2\pi G\sigma/k$. The term proportional to $\beta$ comes from perturbing the density-dependent background shear stress $T_{xy}=-\nu\Sigma S$.

Eliminating $\sigma,u,v$ and using $S=3\Omega/2$, so that the [radial epicyclic frequency](../../../../../../radial-epicyclic-frequency.md) obeys $\kappa_r^2=2\Omega(2\Omega-S)=\Omega^2$, gives the [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{
(\lambda+\nu k^2)
\left\{\lambda\left[\lambda+
\left(\nu_b+\frac43\nu\right)k^2\right]
-2\pi G\Sigma_0k+v_s^2k^2\right\}
+\lambda\Omega^2+3\beta\Omega^2\nu k^2=0}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
