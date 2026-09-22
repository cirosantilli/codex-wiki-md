<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Place a straight coast at $x=0$, ocean at $x<0$, and impose no normal flow at the wall. A coastal Kelvin mode has $u=0$ throughout. The zonal momentum equation becomes $g\eta_x=f_0v$, while the remaining two equations are $v_t+g\eta_y=0$ and $\eta_t+Hv_y=0$. Eliminating $v$ gives

$$
\eta_{tt}=gH\eta_{yy}.
$$

For a northward disturbance $\eta=A(x)F(y-ct)$, the nontrivial solution has $c^2=gH$ and $v=(c/H)\eta$. In the northern hemisphere choose $c=+\sqrt{gH}$; then cross-shore [geostrophic balance](../../../../geostrophic-balance.md) requires

$$
\frac{dA}{dx}=\frac{f_0}{c}A,\qquad
\boxed{A(x)=A_0e^{f_0x/c},\quad c=\sqrt{gH}.}
$$

It decays into this ocean half-plane because $x<0$ and $f_0>0$. The decay length is the external [Rossby deformation radius](../../../../rossby-deformation-radius.md) $L_R=c/f_0$. A Fourier component has $\omega=ck$, so both phase and alongshore group speed are $c$, independent of [wavenumber](../../../../wavenumber.md): the ideal shallow-[water](../../../../water.md) [Kelvin wave](../../../../kelvin-wave.md) is nondispersive.

The signed choice is part of the [boundary condition](../../../../boundary-condition.md). For ocean at $x>0$ in the same hemisphere, decay instead selects southward speed $-\sqrt{gH}$ and $A\propto e^{-f_0x/\sqrt{gH}}$. Without stating the ocean side, an exponential growth into the sea could be mistaken for a trapped coastal mode.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
