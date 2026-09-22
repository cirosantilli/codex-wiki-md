<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For a differentiable [central potential](../../../central-potential.md), the [force](../../../force-split.md) is $\mathbf F=-V'(r)\hat{\mathbf r}$. The [angular momentum](../../../angular-momentum.md) is $\mathbf J=m\mathbf r\times\dot{\mathbf r}$, so

$$
\frac{d\mathbf J}{dt}=\mathbf r\times\mathbf F=0.
$$

This proves [conservation of angular momentum](../../../conservation-of-angular-momentum.md). For $J\ne0$, the trajectory lies in the fixed plane perpendicular to $\mathbf J$. In plane [polar coordinates](../../../polar-coordinates.md), $J=mr^2\dot\phi$. Substituting this into the [kinetic energy](../../../kinetic-energy.md) gives the radial [energy](../../../energy-split.md) equation

$$
E=\frac12m\dot r^2+V_{\mathrm{eff}}(r),\qquad
\boxed{V_{\mathrm{eff}}(r)=V(r)+\frac{J^2}{2mr^2}.}
$$

The second term is the centrifugal contribution to the [effective potential](../../../effective-potential.md). Its radial derivative reproduces $m\ddot r=-V'(r)+J^2/(mr^3)$. Purely radial motion is the $J=0$ case.

For the satellite, write $\mu=GM$, with $M$ Earth's mass and $m$ the satellite's mass. At [apogee](../../../apogee.md) and [perigee](../../../perigee.md), the radial [velocity](../../../velocity.md) is zero, so [angular momentum conservation](../../../conservation-of-angular-momentum.md) and [conservation of energy](../../../conservation-of-energy.md) give

$$
r_{\mathrm A}v_{\mathrm A}=r_{\mathrm P}v_{\mathrm P},\qquad
\frac12v_{\mathrm A}^2-\frac{\mu}{r_{\mathrm A}}
=\frac12v_{\mathrm P}^2-\frac{\mu}{r_{\mathrm P}}.
$$

Eliminating $v_{\mathrm P}$ yields

$$
v_{\mathrm A}^2=\frac{2\mu r_{\mathrm P}}{r_{\mathrm A}(r_{\mathrm A}+r_{\mathrm P})}.
$$

For an [elliptic orbit](../../../elliptic-orbit.md), $r_{\mathrm A}+r_{\mathrm P}=2a$. Therefore the [vis-viva equation](../../../vis-viva-equation.md) at [apogee](../../../apogee.md) is

$$
\boxed{v_{\mathrm A}^2=GM\left(\frac2{r_{\mathrm A}}-\frac1a\right).}
$$

Substitution into the [orbital energy](../../../orbital-energy.md) gives $E=-GMm/(2a)$. The circular case follows by continuity, or directly from the radial [force balance](../../../force-balance.md).

An instantaneous tangential retrograde burn at [apogee](../../../apogee.md) leaves the position unchanged. For the speed change $v\mapsto(1-\epsilon)v$, the [orbital energy](../../../orbital-energy.md) change is

$$
\Delta E=\frac12m\left((1-\epsilon)^2-1\right)v^2
=-\epsilon mv^2+O(\epsilon^2).
$$

Differentiating $E=-\mu m/(2a)$ gives $\Delta E=\mu m\,\Delta a/(2a^2)$ to first order. Since $r_{\mathrm A}=a(1+e)$, the [vis-viva equation](../../../vis-viva-equation.md) implies $v^2=\mu(1-e)/[a(1+e)]$. Hence

$$
\Delta a=-2\epsilon a\frac{1-e}{1+e}+O(\epsilon^2),\qquad
\boxed{\text{reduction of the major axis}= -2\Delta a
=4\epsilon a\frac{1-e}{1+e}+O(\epsilon^2).}
$$

The factor of two distinguishes the major axis from the [semimajor axis](../../../semi-major-axis.md). As a finite-change check, the new [semimajor axis](../../../semi-major-axis.md) is exactly

$$
a'=\frac{a}{1+(2\epsilon-\epsilon^2)(1-e)/(1+e)},
$$

within the instantaneous-burn, unchanged-mass model. Expanding this expression gives the stated result.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2018](../../2018-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
