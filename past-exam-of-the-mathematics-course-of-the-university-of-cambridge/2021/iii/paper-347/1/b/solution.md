<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) $(R,\phi,z)$, put $s=(R^2+z^2)^{1/2}$, and write the purely azimuthal velocity as $\mathbf u=R\Omega\mathbf e_\phi$. The steady radial, azimuthal, and vertical momentum equations are

$$
0=-\frac1\rho\frac{\partial p}{\partial R}
-\frac{GM_{\rm BH}R}{s^3}+R\Omega^2,
\qquad
0=-\frac1{\rho R}\frac{\partial p}{\partial\phi},
$$



$$
0=-\frac1\rho\frac{\partial p}{\partial z}
-\frac{GM_{\rm BH}z}{s^3}.
$$

Thus $\nabla p=\rho\mathbf g_{\rm eff}$, where the [effective gravity in a rotating frame](../../../../../../effective-gravity-in-a-rotating-frame.md) is

$$
\boxed{\mathbf g_{\rm eff}
=-\frac{GM_{\rm BH}}{s^3}(R\mathbf e_R+z\mathbf e_z)
+R\Omega^2\mathbf e_R}.
$$

When [radiation pressure](../../../../../../radiation-pressure.md) supplies the pressure support, force balance gives

$$
\boxed{\frac\kappa c\mathbf F+\mathbf g_{\rm eff}=0,
\qquad
\mathbf F=-\frac c\kappa\mathbf g_{\rm eff}}.
$$

On the upper conical surface $z=R\tan\alpha$, the tangent and outward normal are

$$
\mathbf t=\cos\alpha\,\mathbf e_R+sin\alpha\,\mathbf e_z,
\qquad
\mathbf n=-\sin\alpha\,\mathbf e_R+cos\alpha\,\mathbf e_z.
$$

Because a pressure surface is an [equipotential surface](../../../../../../equipotential-surface.md), $\mathbf g_{\rm eff}\cdot\mathbf t=0$. Since $s=R/\cos\alpha$, this fixes

$$
R\Omega^2=\frac{GM_{\rm BH}\cos\alpha}{R^2},
\qquad
\boxed{\mathbf g_{\rm eff}
=-\frac{GM_{\rm BH}}{R^2}sin\alpha\cos\alpha\,\mathbf n}.
$$

The lower face gives the reflected result. One face has area element $dA=2\pi R,dR/\cos\alpha$. Adding both faces and using $F=c|\mathbf g_{\rm eff}|/\kappa$ yields

$$
dL=2F,dA
=\frac{4\pi GM_{\rm BH}c}{\kappa}
\sin\alpha\frac{dR}{R}.
$$

Consequently

$$
\boxed{L_{\max}=L_{\rm Edd}\sin\alpha
\log\frac{R_2}{R_1}}.
$$

For a broad radial range, each logarithmic interval can radiate an Eddington-scale contribution because rotation reduces the surface-normal gravity. The factor $\sin\alpha$ makes a thin wedge faint and lets a geometrically thick funnel expose a larger effective gravity and emitting area.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
