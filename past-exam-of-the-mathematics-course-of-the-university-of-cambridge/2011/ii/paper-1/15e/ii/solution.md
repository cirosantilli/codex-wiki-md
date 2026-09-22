<h1 id="15e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Normalize the [scale factor](../../../../../../scale-factor-cosmology.md) by $a(t_0)=1$. Separate conservation for a constant equation-of-state parameter $w$ gives $d\log\rho_i=-3(1+w_i)d\log a$. Thus radiation has $\rho_R=\rho_{R0}a^{-4}$ while the [dark energy](../../../../../../dark-energy.md) component with $w=-1$ has constant density. Flatness gives $\Omega_{R0}+\Omega_{\Lambda0}=1$, so

$$
\boxed{\rho(t)=\frac{3H_0^2}{8\pi G}
\left(\frac{\Omega_{R0}}{a^4}+\Omega_{\Lambda0}\right)
=\frac{3H_0^2}{8\pi G}\frac{\Omega_{R0}}{a^4}
\left[1+\frac{1-\Omega_{R0}}{\Omega_{R0}}a^4\right].}
$$

Here $\rho$ has mass-density units in the stated [Friedmann equation](../../../../../../friedmann-equations.md); the corresponding energy density is $\rho c^2$.

Assume both density parameters are positive and choose the Big Bang at $t=0$. The expanding branch satisfies $\dot a=H_0\sqrt{\Omega_{R0}a^{-2}+\Omega_{\Lambda0}a^2}$. Set $u=a^2$ and integrate:

$$
\dot u=2H_0\sqrt{\Omega_{R0}+\Omega_{\Lambda0}u^2},\qquad
\operatorname{arsinh}\left(u\sqrt{\frac{\Omega_{\Lambda0}}{\Omega_{R0}}}\right)
=2H_0\sqrt{\Omega_{\Lambda0}}\,t.
$$

Consequently

$$
\boxed{a(t)=\left(\frac{\Omega_{R0}}{\Omega_{\Lambda0}}\right)^{1/4}
\left[\sinh(2H_0\sqrt{\Omega_{\Lambda0}}\,t)\right]^{1/2},\quad
\alpha=\left(\frac{\Omega_{R0}}{\Omega_{\Lambda0}}\right)^{1/4},\quad
\beta=2H_0\sqrt{\Omega_{\Lambda0}}.}
$$

The factor $H_0$ is required because $\beta$ has inverse-time units. As $t\downarrow0$, $a(t)\sim(2H_0\sqrt{\Omega_{R0}}\,t)^{1/2}$, the expected radiation-dominated power law. As $t\to\infty$, $a(t)\sim\alpha e^{H_0\sqrt{\Omega_{\Lambda0}}t}/\sqrt2$, the exponential expansion driven by a [cosmological constant](../../../../../../cosmological-constant.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [15E](../../15e.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
