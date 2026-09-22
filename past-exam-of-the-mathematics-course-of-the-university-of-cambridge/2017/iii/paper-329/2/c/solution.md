<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $A=R_e^2-R_i^2$, $S=R_e+R_i$, $D=R_e-R_i$, and $Q=Aw=A(0)w_0$. Locally replace $E$ in the preceding [annular viscous extension](../../../../../../annular-viscous-extension.md) calculation by $w'(z)$. Its leading [pressure](../../../../../../pressure.md) is

$$
p=p_e-\frac{(p_i-p_e)R_i^2}{A}+\frac{\gamma S}{A}-\mu w'.
$$

The axial liquid stress relative to ambient [pressure](../../../../../../pressure.md), together with the two circumferential [surface tension](../../../../../../surface-tension.md) [forces](../../../../../../force.md), transmits a cut [force](../../../../../../force.md)

$$
T_{\rm cut}/\pi=3\mu Aw'+(p_i-p_e)R_i^2+\gamma S.
$$

It would be incorrect simply to differentiate this and retain an extra gas-pressure term. The sloping inner gas interface also exerts an axial [pressure](../../../../../../pressure.md) [force](../../../../../../force.md) $-\pi(p_i-p_e)(R_i^2)'$ per unit height, after subtracting the common ambient [pressure](../../../../../../pressure.md) contribution. For constant gas [pressures](../../../../../../pressure.md) these terms cancel. The resulting [capillary tensile force of a hollow slender thread](../../../../../../capillary-tensile-force-of-a-hollow-slender-thread.md) therefore gives

$$
\boxed{3\mu(Aw')'+\rho gA+\gamma S'=0,\qquad Aw=Q.}
$$

Thus the printed axial equation holds even for unequal constant gas [pressures](../../../../../../pressure.md); their influence remains in the radial evolution.

For equal [pressures](../../../../../../pressure.md), the [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) from the previous calculation becomes $wD'=-w'D/2+\gamma/(2\mu)$. Multiplying by the appropriate [integrating factor](../../../../../../integrating-factor.md) gives

$$
\frac d{dz}(D\sqrt w)=\frac{\gamma}{2\mu\sqrt w},\qquad
D(z)\sqrt{w(z)}=D(0)\sqrt{w_0}+\frac\gamma{2\mu}\int_0^z\frac{d\zeta}{\sqrt{w(\zeta)}}.
$$

At closure $R_i=0$, so $D=\sqrt A$ and $D\sqrt w=\sqrt Q$. Hence

$$
\boxed{\frac{\gamma}{2\mu\sqrt{w_0}}\int_0^{z_*}\frac{d\zeta}{\sqrt{w(\zeta)}}=\sqrt{A(0)}-R_e(0)+R_i(0).}
$$

The right side is positive for a genuine annulus. On the gravity-driven quadratic family from the previous part, $w^{1/2}$ grows linearly with height and this [integral](../../../../../../integral.md) diverges logarithmically. It must then reach the finite positive threshold at a finite height. This explains the expected [capillary closure of a falling hollow thread](../../../../../../capillary-closure-of-a-falling-hollow-thread.md) on that freely falling branch without requiring its full coupled profile.

There is a real boundary-data limitation to that expectation. Neither the printed nozzle speed nor the local equations alone guarantee finite closure for every imposed nozzle tension. To see this within the same leading model, define $T=3\mu Qw'/w+\gamma S$, so $T'=-\rho gQ/w$. For equal [pressures](../../../../../../pressure.md) and $w'>0$, both radii decrease and $S\leq S_0$. If

$$
c=\frac{T_0/2-\gamma S_0}{3\mu Q}>0,\qquad
\frac{\rho gQ}{cw_0}<\frac{T_0}{2},
$$

then a bootstrap gives $T>T_0/2$ and $w\geq w_0e^{cz}$: the maximum accumulated weight is smaller than the assumed tension margin. Consequently the closure [integral](../../../../../../integral.md), including its prefactor, is at most $\gamma/(\mu cw_0)$. If this is smaller than $\sqrt{A_0}-D_0$, closure never occurs at finite height. For example, in consistent units choose $\mu=\rho g=w_0=1$, $R_i(0)=\lambda$, $R_e(0)=2\lambda$, $\gamma=\lambda$, $T_0=100\lambda^2$. Then $c=47/9$, the weight bound is $27\lambda^2/47<50\lambda^2$, and $9\lambda/47<(\sqrt3-1)\lambda$. Small $\lambda$ makes the initial geometry slender. Thus **finite closure is the expected freely falling branch behaviour, not a theorem following from nozzle speed alone**. If $\gamma=0$ there is no capillary closure by this mechanism.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
