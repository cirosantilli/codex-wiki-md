<h1 id="section-b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The original diagram has a horizontal bottle neck, so weight does not enter the axial [force](../../../../force-split.md) balance. Gauge pressure acts on the cork's end area and supplies outward [force](../../../../force-split.md) $F_g=\pi a^2P_g$. The radial contact [force](../../../../force-split.md) is the contact pressure times the cylindrical contact area, $N=2\pi a(l-x)P_c$. The limiting friction is $\mu N$, so outward sliding occurs when

$$
\pi a^2P_g>2\pi a(l-x)\mu P_c,\qquad \boxed{P_g>\frac{2(l-x)\mu P_c}{a}.}
$$

The assumption of equal static and [kinetic friction](../../../../kinetic-friction.md) coefficients removes a separate [force](../../../../force-split.md) drop when slipping starts.

Initially the pressure is marginal at $x=0$, so $\pi a^2P_g=2\pi al\mu P_c$. During extraction the contact length decreases, while the pressure [force](../../../../force-split.md) stays constant. The net [force](../../../../force-split.md) is therefore $F(x)=\pi a^2P_gx/l$. The cork's [mass](../../../../mass.md) is $m_c=\rho\pi a^2l$, giving the [pressure-driven cork ejection](../../../../pressure-driven-cork-ejection.md) equation

$$
\boxed{\ddot x=b^2x,\qquad b^2=\frac{P_g}{\rho l^2}.}
$$

For $x(0)=0$ and $\dot x(0)=v_0>0$, solving the constant-coefficient equation gives

$$
\boxed{x(t)=c\sinh(bt),\qquad b=\frac1l\sqrt{\frac{P_g}{\rho}},\qquad c=\frac{v_0}{b}=v_0l\sqrt{\frac\rho{P_g}}.}
$$

The equilibrium is unstable: as the cork moves out, friction decreases and the unbalanced [force](../../../../force-split.md) grows.

Multiplying the equation of motion by $\dot x$ and integrating gives $\dot x^2=v_0^2+b^2x^2$. The contact ends at $x=l$, so

$$
\boxed{v_{\mathrm{exit}}^2=v_0^2+\frac{P_g}{\rho},\qquad v_{\mathrm{exit}}\longrightarrow\sqrt{\frac{P_g}{\rho}}\quad(v_0\to0^+).}
$$

Equivalently, the net [work](../../../../work.md) is $\int_0^lF(x)dx=\pi a^2P_gl/2$. Exactly zero initial [velocity](../../../../velocity.md) would leave the ideal marginal configuration stationary. The exit time $b^{-1}\operatorname{arsinh}(bl/v_0)$ diverges as $v_0\to0^+$, even though the limiting exit [speed](../../../../speed.md) is finite.

The density is $500\,\mathrm{kg\,m^{-3}}$, so $v_{\mathrm{exit}}\simeq\sqrt{400000/500}=28.3\,\mathrm{m\,s^{-1}}$. For an ideal upward launch at this [speed](../../../../speed.md), [conservation of mechanical energy](../../../../conservation-of-mechanical-energy.md) gives height above the exit

$$
\boxed{h=\frac{v_{\mathrm{exit}}^2}{2g}=\frac{P_g}{2\rho g}\simeq40.8\,\mathrm m\approx41\,\mathrm m.}
$$

This neglects air resistance and the small gravitational [work](../../../../work.md) during extraction compared with the launch [energy](../../../../energy-split.md). Actual gas pressure need not stay constant, so it is an idealized estimate.

Adding a stopper that doubles the moving [mass](../../../../mass.md), while preserving the same pressured area and contact friction, leaves the extraction [work](../../../../work.md) unchanged. The squared exit [speed](../../../../speed.md) and the ballistic height are therefore halved:

$$
\boxed{v_{\mathrm{stopper}}=\frac{v_{\mathrm{exit}}}{\sqrt2},\qquad h_{\mathrm{stopper}}=\frac h2\simeq20.4\,\mathrm m.}
$$

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Section B](../../section-b.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
