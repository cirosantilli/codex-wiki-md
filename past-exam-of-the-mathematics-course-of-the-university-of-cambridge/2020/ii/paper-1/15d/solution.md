<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

Take a fixed comoving region, whose physical volume is $V=V_0a^3$. Its energy is $E=\rho V$, so the first-law relation $dE=-P\,dV$ gives

$$
d(\rho a^3)=-P\,d(a^3).
$$

Differentiating with respect to [cosmic time](../../../../../cosmic-time.md) and using the [Hubble parameter](../../../../../hubble-parameter.md) $H=\dot a/a$ yields the [cosmological perfect-fluid continuity equation](../../../../../cosmological-perfect-fluid-continuity-equation.md)

$$
a^3\dot\rho+3a^2\dot a\rho=-3a^2\dot aP,
\qquad
\boxed{\dot\rho=-3H(\rho+P)}.
$$

For the [barotropic equation of state](../../../../../barotropic-equation-of-state.md) $P=w\rho$, separation gives the [constant-equation-of-state density scaling](../../../../../constant-equation-of-state-density-scaling.md)

$$
\rho=\rho_0\left(\frac a{a_0}\right)^{-3(1+w)}.
$$

Substituting this into the flat [Friedmann equation](../../../../../friedmann-equations.md) and integrating the expanding branch gives, for $w\ne-1$,

$$
\boxed{a(t)\propto(t-t_*)^{2/[3(1+w)]}}.
$$

For $w=-1$, the density and [Hubble parameter](../../../../../hubble-parameter.md) are constant and instead $a(t)\propto e^{Ht}$.

[Conformal time](../../../../../conformal-time.md) is defined by

$$
d\tau=\frac{dt}{a(t)},
\qquad
\frac{da}{d\tau}=a\dot a=a^2H.
$$

At radiation–string equality, let each component have density $\rho_{\rm eq}$ at $a=a_{\rm eq}$. Since [radiation in cosmology](../../../../../radiation-in-cosmology.md) has $w=1/3$ and a [cosmic string network](../../../../../cosmic-string-network.md) has $w=-1/3$,

$$
\rho_r=\rho_{\rm eq}\left(\frac{a_{\rm eq}}a\right)^4,
\qquad
\rho_s=\rho_{\rm eq}\left(\frac{a_{\rm eq}}a\right)^2.
$$

Consequently

$$
\left(\frac{da}{d\tau}\right)^2
=a^4\frac{8\pi G}{3c^2}(\rho_r+\rho_s)
=\frac{8\pi G a_{\rm eq}^2}{3c^2}\rho_{\rm eq}
(a^2+a_{\rm eq}^2).
$$

Thus

$$
\boxed{B=\frac{8\pi G a_{\rm eq}^2}{3c^2}}.
$$

On the expanding branch, integration gives

$$
\operatorname{arsinh}\!\left(\frac a{a_{\rm eq}}\right)
=\sqrt{B\rho_{\rm eq}}\,(\tau-\tau_0).
$$

Choosing the Big Bang to occur at $\tau=0$ gives the [radiation--cosmic-string Friedmann solution](../../../../../radiation-cosmic-string-friedmann-solution.md)

$$
\boxed{a(\tau)=a_{\rm eq}\sinh\!\left(\sqrt{B\rho_{\rm eq}}\,\tau\right)}.
$$

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
