<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the length convention $\ell_m=-U_*^3/B_0$; a dimensionless multiplier can be absorbed into the similarity functions. [Dimensional analysis](../../../../../../dimensional-analysis.md) under the stated local dependence gives

$$
K_M=U_*z f_M(\zeta),\qquad K_B=U_*z f_B(\zeta),\qquad \zeta=z/\ell_m.
$$

To obtain a log-linear expansion one also needs a regular neutral limit: take $f_M=a_M+d_M\zeta+O(\zeta^2)$ and $f_B=a_B+d_B\zeta+O(\zeta^2)$, with positive $a_M,a_B$. Dimensions alone do not specify these constants or guarantee differentiability. Let $s_u=-J_M/U_*^2$ denote the shear sign. In the high-number regime of part (a), integrate the reciprocal expansions from a reference height $z_r>0$ to obtain the [near-neutral log-linear surface-layer profiles](../../../../../../near-neutral-log-linear-surface-layer-profiles.md)

$$
\boxed{\bar u(z)-\bar u(z_r)=\frac{s_uU_*}{a_M}
\left[\ln\frac z{z_r}-\frac{d_M}{a_M}\frac{z-z_r}{\ell_m}+O(\zeta^2+\zeta_r^2)\right],}
$$



$$
\boxed{\bar b(z)-\bar b(z_r)=-\frac{B_0}{a_BU_*}
\left[\ln\frac z{z_r}-\frac{d_B}{a_B}\frac{z-z_r}{\ell_m}+O(\zeta^2+\zeta_r^2)\right].}
$$

Their leading terms are logarithmic; the first buoyancy-dependent corrections are linear in height. The additive constants require boundary or reference data and cannot be obtained from the prescribed fluxes alone.

The [gradient Richardson number](../../../../../../gradient-richardson-number.md) is

$$
\boxed{\mathrm{Ri}=\frac{\bar b_z}{\bar u_z^2}=-\frac{B_0z}{U_*^3}\frac{f_M^2}{f_B}
=\frac z{\ell_m}\frac{f_M^2}{f_B}.}
$$

Thus $|z/\ell_m|\ll1$ is nearly neutral, shear-dominated turbulence: the buoyancy contribution is small relative to shear production. Stable flux has $B_0<0$, $\ell_m>0$ and positive Richardson number; heating has $B_0>0$, $\ell_m<0$ and negative Richardson number. The smallness condition is on the magnitude, not an automatically satisfied signed inequality for every negative $z/\ell_m$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
