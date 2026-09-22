<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the usual spherical [circular-shell adiabatic contraction](../../../../../../circular-shell-adiabatic-contraction.md) approximation: initial dark-matter orbits are circular, slow accumulation keeps them circular, and dark shells do not cross. [Angular momentum](../../../../../../angular-momentum.md) is conserved in a spherical potential, and the vanishing [radial action](../../../../../../radial-action.md) stays zero as an [adiabatic invariant](../../../../../../adiabatic-invariant.md). For a circular shell,

$$
L^2=GrM(r),\qquad r_iM_i(r_i)=rM_f(r).
$$

Here $r_i$ is the initial shell radius and $r$ its final radius. The final flat [circular speed](../../../../../../circular-speed.md) $V=2v_{\rm NFW,c,max}$ gives $M_f(r)=V^2r/G$.

For an initial shell in the inner [NFW profile](../../../../../../navarro-frenk-white-profile.md), write $A=2\pi\rho_1r_1$, so $M_i(r_i)\simeq Ar_i^2$. The invariant gives

$$
Ar_i^3=\frac{V^2}G r^2,
\qquad r_i=\left(\frac{V^2}{GA}\right)^{1/3}r^{2/3}.
$$

Conservation of dark shell mass yields

$$
M'_D(r)=Ar_i^2=A^{1/3}\left(\frac{V^2}G\right)^{2/3}r^{4/3},
$$

and differentiation gives

$$
\rho'_D(r)=\frac{A^{1/3}}{3\pi}\left(\frac{V^2}G\right)^{2/3}r^{-5/3}.
$$

To express the requested ratios, set $K=F(x_{\max})\simeq0.2162166$ and $B=8K\simeq1.72973$, so $V^2/(GA)=Br_1$. Since the original cusp has $\rho_D(r)\simeq A/(2\pi r)$,

$$
\boxed{f(r)\simeq\frac23\left(\frac{Br_1}r\right)^{2/3}
\simeq0.96064\left(\frac{r_1}r\right)^{2/3}.}
$$

The total density of the final spherical flat-rotation model is $\rho_{\rm tot}=V^2/(4\pi Gr^2)$. Its dark fraction is

$$
h(r)\equiv\frac{\rho'_D}{\rho_{\rm tot}}
\simeq\frac43\left(\frac r{Br_1}\right)^{1/3}.
$$

Subtracting dark matter from the total gives the added-matter density, $\rho_B=\rho_{\rm tot}(1-h)$, and thus

$$
\boxed{g(r)\simeq\frac{\tfrac43(r/(Br_1))^{1/3}}
{1-\tfrac43(r/(Br_1))^{1/3}}
\sim1.11074\left(\frac r{r_1}\right)^{1/3}.}
$$

These expressions describe the leading inner approximation, not an extension to radii where the denominator becomes negative or the initial shell is outside the NFW cusp. As $r/r_1\to0$, dark matter is enhanced relative to its original density while its fraction of the even steeper total density tends to zero. This is [inner NFW contraction to a flat rotation curve](../../../../../../inner-nfw-contraction-to-a-flat-rotation-curve.md).

**The orbital assumptions matter.** An initial density profile does not specify the [phase-space distribution function](../../../../../../phase-space-distribution-function.md). For eccentric orbits, slow evolution conserves their actions, but $rM(r)$ at an instantaneous radius is not generally their invariant. The above ratios are the intended circular-shell estimate; their numerical coefficients cannot be uniquely inferred from the density profile and slow accumulation alone.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
