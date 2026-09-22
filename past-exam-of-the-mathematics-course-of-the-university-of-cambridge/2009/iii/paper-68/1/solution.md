<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $\dot M>0$ to mean inward [accretion rate](../../../../../accretion-rate.md), and let $S$ count loss through both faces per unit projected area of the [accretion disk](../../../../../accretion-disk.md). An annulus of width $dR$ loses $2\pi R S\,dR$ to the wind. In steady state, its incoming mass flux at its outer edge equals the inward flux at its inner edge plus this loss. Hence [mass conservation](../../../../../mass-conservation.md) gives

$$
\boxed{\frac{d\dot M}{dR}=2\pi RS.}
$$

If a loss rate is instead defined per individual face, it must be doubled before substituting for $S$ here.

Use [Keplerian rotation](../../../../../keplerian-disk.md) $\Omega^2=GM/R^3$. The vertically integrated [viscous dissipation](../../../../../viscous-dissipation.md), summed over both disk faces, is

$$
Q^+=\nu\Sigma\left(R\frac{d\Omega}{dR}\right)^2=\frac94\nu\Sigma\Omega^2.
$$

Here $\nu$ is the [kinematic viscosity](../../../../../kinematic-viscosity.md), and $\Sigma$ is the [surface density of a disk](../../../../../surface-density-of-a-disk.md); for height-dependent viscosity the product means $\int\rho\nu\,dz$. Material already in a circular orbit has [specific orbital energy](../../../../../specific-orbital-energy.md) $v_K^2/2-GM/R=-GM/(2R)$. Giving it zero total binding energy therefore costs an additional $GM/(2R)$ per unit mass. The total launch speed is the [escape velocity](../../../../../escape-velocity.md) $\sqrt{2GM/R}$, but one must not charge the wind for the orbital [kinetic energy](../../../../../kinetic-energy.md) it already possesses. Equating wind power to $fQ^+$ gives

$$
f\frac94\nu\Sigma\frac{GM}{R^3}=S\frac{GM}{2R}.
$$

Combining this with [mass conservation](../../../../../mass-conservation.md) yields the [wind-powered mass loss from a steady accretion disk](../../../../../wind-powered-mass-loss-from-a-steady-accretion-disk.md) relation

$$
\boxed{\nu\Sigma=\frac{2SR^2}{9f}=\frac{R}{9\pi f}\frac{d\dot M}{dR}.}
$$

Define the outward [viscous torque in an accretion disk](../../../../../viscous-torque-in-an-accretion-disk.md) as

$$
\mathcal G=-2\pi R^3\nu\Sigma\frac{d\Omega}{dR}=3\pi\nu\Sigma h,\qquad h=R^2\Omega=\sqrt{GMR}.
$$

The net inward [angular momentum](../../../../../angular-momentum.md) flux is $\dot Mh-\mathcal G$. Because each unit mass lost to the wind carries the local [specific angular momentum](../../../../../specific-angular-momentum.md) $h$, annular [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) reads

$$
\frac{d}{dR}(\dot Mh-\mathcal G)=h\frac{d\dot M}{dR},\qquad
\mathcal G'=\dot M h'=\frac{\dot M h}{2R}.
$$

In the wind region, $\mathcal G=Rh\dot M'/(3f)$. For constant $f$, differentiation and cancellation of $h$ gives

$$
R\dot M''+\frac32\dot M'=\frac{3f}{2R}\dot M.
$$

Thus the requested [Cauchy-Euler differential equation](../../../../../cauchy-euler-equation.md) is

$$
\boxed{R^{1/2}\frac{d}{dR}\left(R^{3/2}\frac{d\dot M}{dR}\right)=\frac32f\dot M.}
$$

For $f=1/3$, a power-law trial $\dot M\propto R^p$ gives $p^2+p/2-1/2=0$, with roots $p=1/2,-1$. Therefore $\dot M=A\sqrt R+B/R$ in $R_*\le R\le R_0$. A zero inner [viscous torque in an accretion disk](../../../../../viscous-torque-in-an-accretion-disk.md) implies $\dot M'(R_*)=0$, so $B=AR_*^{3/2}/2$. There is no point mass sink at $R_0$, so the [accretion rate](../../../../../accretion-rate.md) is continuous there and equals $\dot M_0$. The complete result is

$$
\boxed{\dot M(R)=\begin{cases}
\displaystyle\dot M_0\frac{\sqrt R+R_*^{3/2}/(2R)}{\sqrt{R_0}+R_*^{3/2}/(2R_0)},&R_*\le R\le R_0,\\
\dot M_0,&R\ge R_0.
\end{cases}}
$$

Its derivative is nonnegative throughout the wind region, as required for a nonnegative loss rate $S$. The derivative can jump to zero outside $R_0$: the energy relation applies only inside the wind zone and does not impose $\dot M'(R_0)=0$ on its inner limit. The [viscous torque in an accretion disk](../../../../../viscous-torque-in-an-accretion-disk.md) remains continuous and extends outside via $\mathcal G'=\dot M_0h'$.

At the inner boundary the exact accreted fraction is

$$
\boxed{\frac{\dot M(R_*)}{\dot M_0}=\frac{\tfrac32\sqrt{R_*/R_0}}{1+\tfrac12(R_*/R_0)^{3/2}}
\simeq\frac32\left(\frac{R_*}{R_0}\right)^{1/2}\quad(R_*\ll R_0).}
$$

The last expression is a leading-order asymptotic equality, not the exact finite-radius fraction. Most of the supplied mass is expelled before reaching the star when $R_*/R_0$ is small.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
