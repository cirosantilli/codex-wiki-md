<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\gamma=5/3$, the shock data give $\rho_{\rm ps}=4\rho_0$ and $u_{\rm ps}=3V_s/4$. Since $V_s=R/(3t)$, the prescribed [homologous spherical flow](../../../../../../homologous-spherical-flow.md) is

$$
u(r,t)=\frac{r}{4t}.
$$

Put $\xi=r/R(t)$ and $\rho=\rho_0D(\xi)$. The spherical [continuity equation](../../../../../../continuity-equation.md) becomes

$$
-\frac{\xi}{3}D'+\frac14(3D+\xi D')=0,
$$

so $D\propto\xi^9$. Matching the post-shock density gives

$$
\rho(r,t)=4\rho_0\xi^9.
$$

The [material acceleration](../../../../../../material-acceleration.md) is

$$
\frac{Du}{Dt}=-\frac{3r}{16t^2}.
$$

The radial [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) thus give $dp/dr=3\rho r/(16t^2)$. Integrating from the centre to the shock,

$$
p_{\rm ps}-p(0,t)
=\frac{3}{16t^2}\int_0^R\rho r\,dr
=\frac{3\rho_0R^2}{44t^2}.
$$

Since $p_{\rm ps}=\rho_0R^2/(12t^2)$,

$$
\boxed{p(0,t)=\frac{\rho_0R^2}{66t^2}
=\frac{2}{11}p_{\rm ps}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
