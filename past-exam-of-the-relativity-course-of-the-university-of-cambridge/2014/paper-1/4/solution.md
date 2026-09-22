<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**[geodesic](../../../../geodesic.md) integrals and affine normalization.** Put $F(r)=1-2\mu/r$. Choose the [affine parameter](../../../../affine-parameter.md) to be [proper time](../../../../proper-time.md), so $g_{ab}\dot x^a\dot x^b=c^2$. Cyclic $t$ and $\phi$ in the [geodesic Lagrangian](../../../../geodesic-lagrangian.md) give $F\dot t=k$ and $r^2\dot\phi=h$. Substituting into the [four-velocity](../../../../four-velocity.md) normalization gives

$$
c^2=\frac{c^2k^2}{F}-\frac{\dot r^2}{F}-\frac{h^2}{r^2},
$$

hence

$$
\boxed{\dot r^2-\frac{2\mu h^2}{r^3}
+\frac{h^2}{r^2}-\frac{2\mu c^2}{r}
=(k^2-1)c^2}.
$$

An arbitrary constant rescaling of [affine parameter](../../../../affine-parameter.md) changes its normalization; the displayed unit constant assumes the proper-time choice.

**[circular orbit](../../../../circular-orbit.md).** Define $V(r)=h^2/r^2-2\mu h^2/r^3-2\mu c^2/r$. The radial [geodesic equation](../../../../geodesic-equation.md) is $\ddot r=-V'/2$. A circular [geodesic](../../../../geodesic.md) therefore needs $V'(R)=0$, not merely $\dot r=0$ at an instant. Solving and substituting into the radial first integral gives

$$
\boxed{h^2=\frac{\mu c^2R^2}{R-3\mu},\qquad
k^2=\frac{(R-2\mu)^2}{R(R-3\mu)}}.
$$

Existence requires $R>3\mu$. [circular orbits](../../../../circular-orbit.md) below $6\mu$ are radially unstable, although they still define the instantaneous comparison here.

**[orthogonal local velocities in Schwarzschild spacetime](../../../../orthogonal-local-velocities-in-schwarzschild-spacetime.md).** Use Alice's static [orthonormal frame](../../../../orthonormal-frame-in-spacetime.md) at the meeting event. Her proper clock is $d\tau_A=\sqrt F\,dt$ and tangential proper distance is $R\,d\phi$. Bob's local tangential speed is

$$
v_{\rm AB}=\frac{R\,d\phi}{\sqrt F\,dt}
=\frac{h\sqrt F}{Rk},
\qquad
\boxed{v_{\rm AB}=c\sqrt{\frac{\mu}{R-2\mu}}}.
$$

Carol has $h_C=0$ and $k_C=1$, because she starts from rest at infinity. The radial integral gives $\dot r_C=-c\sqrt{2\mu/R}$. Her static-frame radial speed is $(dr/\sqrt F)/(\sqrt F\,dt)=dr/(Fdt)$, and $F\dot t_C=1$, so

$$
\boxed{v_{\rm AC}=c\sqrt{\frac{2\mu}{R}}}.
$$

This is inward radial motion, perpendicular to Bob's tangential motion in Alice's frame.

Their [Lorentz factors](../../../../lorentz-factor.md) relative to Alice are $\gamma_{\rm AB}=\sqrt{(R-2\mu)/(R-3\mu)}$ and $\gamma_{\rm AC}=\sqrt{R/(R-2\mu)}$. The [four-velocity](../../../../four-velocity.md) contraction therefore gives

$$
\gamma_{\rm BC}=\gamma_{\rm AB}\gamma_{\rm AC}
=\sqrt{\frac{R}{R-3\mu}},\qquad
\boxed{v_{\rm BC}=c\sqrt{\frac{3\mu}{R}}}.
$$

**Special-relativistic consistency.** Let Bob's tangential [velocity](../../../../velocity.md) in Alice's local frame be $u$ and Carol's inward radial speed be $w$. A boost to Bob's frame gives Carol components $v'_{\rm tang}=-u$ and $v'_{\rm rad}=-w/\gamma_u$. Consequently

$$
\frac{v_{\rm BC}^2}{c^2}
=\frac{u^2}{c^2}+\frac{w^2}{c^2}
-\frac{u^2w^2}{c^4}
=\frac{\mu}{R-2\mu}+\frac{2\mu}{R}
-\frac{2\mu^2}{R(R-2\mu)}
=\frac{3\mu}{R}.
$$

Thus the three measured relative speeds agree with local Lorentz [velocity](../../../../velocity.md) addition. Ordinary Euclidean subtraction of the two [velocity](../../../../velocity.md) vectors would omit the transverse-velocity transformation.

<a id="4/image-original-local-frame-velocity-comparison-for-static-circular-and-infalling-observers"></a>
![](../../../../past-exam-of-the-relativity-course-of-the-university-of-cambridge/2014/paper-1-local-relative-velocities.png)

**[Figure 2](#4/image-original-local-frame-velocity-comparison-for-static-circular-and-infalling-observers). Original local-frame velocity comparison for static, circular and infalling observers**.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
