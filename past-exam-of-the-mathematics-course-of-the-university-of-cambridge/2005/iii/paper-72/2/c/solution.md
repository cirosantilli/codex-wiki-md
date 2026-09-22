<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Inside the uniform sphere, $V_c^2=3\sigma^2r^2/r_0^2$. Thus, with $X=V_c/(\sqrt2\sigma)$, part (b) gives

$$
\frac{v_e^2}{2\sigma^2}=\frac92-X^2,\qquad 0\leq X\leq\sqrt{3/2}.
$$

The [Gaussian integral](../../../../../../gaussian-integral.md) needed for the [lowered Maxwellian velocity distribution](../../../../../../lowered-maxwellian-velocity-distribution.md) is

$$
\int_0^X y^2e^{-y^2}\,dy=\frac{\sqrt\pi}4\operatorname{erf}X-\frac X2e^{-X^2}.
$$

Substitution $v=\sqrt2\sigma y$ therefore yields

$$
\int_0^{V_c}f(v)v^2\,dv=n_0I(X),\qquad I(X)=\frac1{4\pi}\left[\operatorname{erf}X-\frac{2X}{\sqrt\pi}e^{-X^2}-\frac{4X^3}{3\sqrt\pi}e^{X^2-9/2}\right].
$$

Since $V_c<v_e$ throughout the core, the integrand is positive and so is $I(X)$ for $X>0$. Using $mn_0=\rho_0$, part (a)'s massive-test-body drag magnitude is

$$
D=-\dot V\big|_{\rm drag}=\frac{16\pi^2G^2M\rho_0\ln\Lambda}{V_c^2}I(X).
$$

The slow drift of a [circular orbit](../../../../../../circular-orbit.md) is determined by [torque](../../../../../../torque.md), not by equating its changing [circular speed](../../../../../../circular-speed.md) to the tangential drag. Here $V_c=\omega r$, with constant $\omega=\sqrt{4\pi G\rho_0/3}$. The [specific angular momentum](../../../../../../specific-angular-momentum.md) $j=rV_c=\omega r^2$ obeys

$$
\dot j=2V_c\dot r=-rD,\qquad \dot r=-\frac{rD}{2V_c}<0.
$$

Hence the positive local decay timescale is

$$
\boxed{\tau_+\equiv\frac{r}{2|\dot r|}=\frac{V_c}{D}=\frac{V_c^3}{16\pi^2G^2M\rho_0\ln\Lambda\,I(X)}.}
$$

There is a genuine factor-of-two discrepancy with the requested denominator $32\pi^2$. That denominator would give $V_c/(2D)$, which is the timescale for a flat [galaxy rotation curve](../../../../../../galaxy-rotation-curve.md), not this uniform-density core. It also follows from the incorrect replacement $\dot V_c=-D$, which drops the $V_c\dot r$ term in $d(rV_c)/dt$. The literal signed definition $r/(2\dot r)$ is negative for an inward drift; it equals $-\tau_+$. A positive decay time requires the absolute value or a minus sign.

This is the [slow circular inspiral under tangential drag](../../../../../../slow-circular-inspiral-under-tangential-drag.md) calculation. Its assumptions require $D$ small enough for nearly circular adjustment and a meaningful large [Coulomb logarithm in stellar dynamics](../../../../../../coulomb-logarithm-in-stellar-dynamics.md); the leading-log approximation is not uniform at $V_c\to0$. Also, integrating the truncated distribution all the way to $v_e$ does not give exactly $n_0$. The model uses $n_0$ as the stated core normalization; exact self-consistency of a sharply truncated uniform core with that distribution is not implied.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
