<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For either component $j\in\{h,s\}$ and $0<\gamma<3$, direct integration of the [power law](../../../../../power-law.md) density gives

$$
\boxed{M_j(<r)=\frac{4\pi A_j}{3-\gamma}r^{3-\gamma}},
\qquad
\boxed{v_{c,j}^2(r)=\frac{GM_j(<r)}r
=\frac{4\pi GA_j}{3-\gamma}r^{2-\gamma}}.
$$

Let $B_j=4\pi GA_j/(3-\gamma)$. Since $d\Phi_j/dr=GM_j/r^2=B_jr^{1-\gamma}$,

$$
\boxed{
\Phi_j(r)=
\begin{cases}
B_jr^{2-\gamma}/(2-\gamma)+C_j,&\gamma\ne2,\\
B_j\log r+C_j,&\gamma=2.
\end{cases}}
$$

The additive constants depend on the chosen reference and cannot generally be set by requiring $\Phi\to0$ at infinity for an untruncated power law.

For a satellite on a circular orbit, the linearized effective radial force gives the [tidal radius](../../../../../tidal-radius.md)

$$
r_t^3=\frac{GM_s(<r_t)}{\Omega^2-\Phi_h''(r_o)}.
$$

Here $\Omega^2=GM_h(<r_o)/r_o^3=B_hr_o^{-\gamma}$ and $\Phi_h''=(1-\gamma)\Omega^2$, so

$$
r_t^3=\frac{GM_s(<r_t)}{\gamma\Omega^2}.
$$

Substitution of the two mass profiles yields

$$
\boxed{\frac{r_t}{r_o}=
\left(\frac{A_s}{\gamma A_h}\right)^{1/\gamma}},
$$

and equivalently

$$
\boxed{\frac{r_t}{r_o}
=\left[\frac{M_s(<r_t)}{\gamma M_h(<r_o)}\right]^{1/3}
\sim\left[\frac{M_s(<r_t)}{M_h(<r_o)}\right]^{1/3}}.
$$

Now set $\gamma=1$. Then

$$
r_t=\frac{A_s}{A_h}r_o,
\qquad
M_s(<r_t)=2\pi A_sr_t^2
=\mu r_o^2,
\qquad
\mu=\frac{2\pi A_s^3}{A_h^2}.
$$

The host circular speed is $v=B\sqrt{r_o}$ with $B=\sqrt{2\pi GA_h}$. The magnitude of [Chandrasekhar dynamical friction](../../../../../chandrasekhar-dynamical-friction.md) becomes

$$
a_{\rm df}
=4\pi G^2M_s\frac{A_h}{r_o}
\frac{\log\Lambda}{B^2r_o}K
=2G\mu K\log\Lambda,
$$

a constant. The specific angular momentum is $j=r_ov=Br_o^{3/2}$. Since the drag torque gives $dj/dt=-r_oa_{\rm df}$,

$$
\frac32B\sqrt{r_o}\frac{dr_o}{dt}
=-r_oa_{\rm df},
$$

and therefore

$$
\boxed{\frac{dr_o}{dt}=-C\sqrt{r_o}},
\qquad
C=\frac{2a_{\rm df}}{3B}>0.
$$

Integration gives

$$
2\sqrt{r_o(t)}=2\sqrt{r_{o0}}-Ct,
\qquad
\boxed{t_{\rm merge}=\frac{2\sqrt{r_{o0}}}{C}},
$$

which is finite.

If stripping is switched off, hold the satellite mass at its initial value $M_0=\mu r_{o0}^2$. The frictional acceleration is then $a_{\rm df}=a_0r_{o0}^2/r_o^2$, where $a_0$ is the constant acceleration in the stripped calculation. The same torque equation gives

$$
\frac{dr_o}{dt}=-Cr_{o0}^2r_o^{-3/2}.
$$

Thus

$$
t_{\rm no\ strip}
=\frac1{Cr_{o0}^2}\int_0^{r_{o0}}r^{3/2}\,dr
=\frac{2\sqrt{r_{o0}}}{5C}
=\boxed{\frac{t_{\rm merge}}5}.
$$

Without [tidal stripping](../../../../../tidal-stripping.md), the satellite retains its mass while the background density increases inward, so dynamical friction strengthens rapidly. Stripping instead gives $M_s\propto r_o^2$ and removes the very mass that creates the gravitational wake.

For a singular isothermal host, $\rho_h=A_hr^{-2}$, $M_h\propto r$, and $v=B$ is constant. The tidal formula with a satellite $\rho_s=A_sr^{-1}$ gives

$$
r_t\propto r_o^2,
\qquad
M_s\propto r_t^2\propto r_o^4.
$$

Consequently $a_{\rm df}\propto M_s\rho_h/v^2\propto r_o^2$. Since now $j=Br_o$, the torque equation yields

$$
\boxed{\frac{dr_o}{dt}=-C_2r_o^3}.
$$

Its solution satisfies $r_o^{-2}=r_{o0}^{-2}+2C_2t$, so $r_o$ approaches zero only as $t^{-1/2}$ and never arrives in finite time. This is [dynamical-friction stalling by tidal stripping](../../../../../dynamical-friction-stalling-by-tidal-stripping.md): the inward tidal field strips the satellite so aggressively that its wake and drag disappear. Observationally, disrupted satellites should deposit stars in streams and the stellar halo, surviving low-mass remnants can remain at finite radii for very long times, and merger times inferred from a constant satellite mass can be severe underestimates.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
