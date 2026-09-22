<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a swept shell, momentum conservation may be written

$$
\frac d{dt}\left[M_{\rm sh}(R)\dot R\right]
=\frac Lc\left(1-e^{-\tau_{\rm UV}}+\tau_{\rm IR}\right)
-\frac{GM_{\rm sh}(R)[M_{\rm BH}+M_h(<R)]}{R^2}
-4\pi R^2P_{\rm ext}.
$$

The first term is direct ultraviolet absorption plus trapped-infrared radiation pressure, the second is gravity from the black hole and host, and the last is external pressure. The derivative also accounts for the inertia of newly swept-up gas.

For a [singular isothermal sphere](../../../../../../singular-isothermal-sphere.md),

$$
M_h(<R)=\frac{2\sigma^2R}{G},
\qquad
M_{\rm sh}=f_{\rm gas}M_h
=\frac{2f_{\rm gas}\sigma^2R}{G}.
$$

Outside the black hole's sphere of influence and with external pressure neglected, gravity is the constant force $4f_{\rm gas}\sigma^4/G$. The shell optical depths are

$$
\tau_i=\frac{\kappa_iM_{\rm sh}}{4\pi R^2}
=\frac{\kappa_if_{\rm gas}\sigma^2}{2\pi GR}.
$$

Thus the [dust transparency radius](../../../../../../dust-transparency-radius.md) and dimensionless optical depths are

$$
R_\tau=\frac{\kappa_{\rm UV}f_{\rm gas}\sigma^2}{2\pi G},
\qquad
\tau_{\rm UV}=\frac1{R'},
\qquad
\tau_{\rm IR}=\frac{\kappa_{\rm IR}}{\kappa_{\rm UV}}\frac1{R'}.
$$

With $R'=R/R_\tau$, $t'=t/t_\tau$, $t_\tau=R_\tau/(\sqrt2\sigma)$, and

$$
L_{\rm crit}=\frac{4f_{\rm gas}c\sigma^4}{G},
\qquad
\xi=\frac L{L_{\rm crit}},
$$

the shell equation becomes

$$
\boxed{\frac d{dt'}\left(R'\frac{dR'}{dt'}\right)
=\xi\left(1-e^{-\tau_{\rm UV}}+\tau_{\rm IR}\right)-1}.
$$

In the optically thick single-scattering regime, $1-e^{-\tau_{\rm UV}}\simeq1$ and $\tau_{\rm IR}$ is neglected. Integrating the constant right-hand side gives

$$
\boxed{(R')^2=(\xi-1)(t')^2
+2R'_0\dot R'_0t'+(R'_0)^2}.
$$

The zero-radius member has $R'=\sqrt{\xi-1}\,t'$ and hence the physical constant speed

$$
\boxed{\dot R=\sqrt{2(\xi-1)}\,\sigma}.
$$

As the shell becomes ultraviolet-thin,

$$
1-e^{-\tau_{\rm UV}}=1-e^{-1/R'}
\simeq\frac1{R'}.
$$

The net force becomes negative beyond the force-balance radius

$$
R'_{\rm dec}=
\left[\log\!\left(\frac{\xi}{\xi-1}\right)\right]^{-1}
\simeq\xi,
$$

but inertia carries the shell farther before it stalls. Match the thick solution at $R'=1$, where $\dot R'^2=\xi-1$. In the thin approximation,

$$
\frac d{dt'}(R'\dot R')=\frac{\xi}{R'}-1.
$$

Using $d/dt'=\dot R' d/dR'$ and integrating gives

$$
(R'\dot R')^2=2\xi R'-(R')^2-\xi.
$$

The outer zero is the stalling radius

$$
\boxed{R'_{\rm stall}=\xi+\sqrt{\xi(\xi-1)}}.
$$

Including the optically thick travel time from a negligible launch radius, the dimensionless stalling time is

$$
t'_{\rm stall}=\frac1{\sqrt{\xi-1}}+\sqrt{\xi-1}
+\xi\left[
\frac\pi2+\sin^{-1}\sqrt{\frac{\xi-1}{\xi}}
\right].
$$

Solving $dt'_{\rm stall}/d\xi=0$ gives $\xi\simeq1.248$, so

$$
\boxed{\epsilon\simeq0.25}.
$$

For $1<\xi<1+\epsilon$, a stronger mildly supercritical source reaches transparency so much sooner that its total stalling time decreases even though it travels farther. Above this range, the increasing coasting distance dominates. Stalling means that loss of ultraviolet optical depth reduces radiation coupling below gravity; without renewed driving, the swept gas falls back or remains bound rather than escaping the halo.

In the infrared multi-scattering regime, the dominant force is $\xi\tau_{\rm IR}=a/R'$ with $a=\xi\kappa_{\rm IR}/\kappa_{\rm UV}$. Seeking $R'=At'^{2/3}$ in

$$
\frac d{dt'}(R'\dot R')=\frac a{R'}
$$

gives $A^3=9a/2$ and therefore

$$
\boxed{\dot R'=
\left(\frac{4\kappa_{\rm IR}\xi}{3\kappa_{\rm UV}}\right)^{1/3}
(t')^{-1/3}}.
$$

Infrared trapping supplies more than the single-scattering momentum while the shell is compact and optically thick. The speed nevertheless decreases as $t'^{-1/3}$ because the shell sweeps up mass and its infrared optical depth falls. Such driving can launch a powerful [dusty radiation-pressure-driven shell](../../../../../../dusty-radiation-pressure-driven-shell.md), but propagation to halo scales requires enough integrated momentum before the shell becomes transparent; otherwise gravity eventually stalls it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
