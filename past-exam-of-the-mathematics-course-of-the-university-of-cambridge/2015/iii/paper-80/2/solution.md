<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $s$ be arclength, $\mathbf t=\partial_s\mathbf r$ the unit tangent, and $\mathbf v$ the local filament velocity relative to the fluid. The [resistive-force theory](../../../../../resistive-force-theory.md) force per unit arclength, exerted by the fluid on the filament, is

$$
\boxed{\mathbf f
=-\xi_\parallel(\mathbf v\cdot\mathbf t)\mathbf t
-\xi_\perp[\mathbf v-(\mathbf v\cdot\mathbf t)\mathbf t]
=-\xi_\perp\mathbf v+
(\xi_\perp-\xi_\parallel)(\mathbf v\cdot\mathbf t)\mathbf t.}
$$

The [parallel and perpendicular drag coefficients of a slender filament](../../../../../parallel-and-perpendicular-drag-coefficients-of-a-slender-filament.md) are proportional to [dynamic viscosity](../../../../../dynamic-viscosity.md). For radius $a$ and a relevant axial cutoff length $\ell\gg a$, the [anisotropic slender-filament drag from Stokeslet integration](../../../../../anisotropic-slender-filament-drag-from-stokeslet-integration.md) gives the leading logarithmic forms

$$
\xi_\parallel\sim\frac{2\pi\mu}{\ln(\ell/a)},\qquad
\xi_\perp\sim\frac{4\pi\mu}{\ln(\ell/a)}.
$$

The cutoff may be set by filament length or deformation wavelength. End shape and the choice of cutoff change order-one constants inside the logarithms. [Slender-body theory](../../../../../slender-body-theory.md) also includes nonlocal interactions that the local [resistive-force theory](../../../../../resistive-force-theory.md) approximation omits. Typically $\xi_\perp>\xi_\parallel$, with ratio tending to two in the slender limit; this drag anisotropy enables propulsion.

Write $C=\xi_\perp-\xi_\parallel>0$. For a small-amplitude planar deformation, $\mathbf t=(1,y_x)+O(y_x^2)$ and the leading transverse velocity is $y_t$. Exact [inextensibility](../../../../../inextensible-filament.md) requires the [quadratic longitudinal displacement of an inextensible planar filament](../../../../../quadratic-longitudinal-displacement-of-an-inextensible-planar-filament.md): if $X(s,t)=s+X_2(s,t)$ and $Y(s,t)=y(s,t)$, then $X_{2,s}=-y_s^2/2$ to this order. Its velocity is quadratic and has zero time average for a periodic material cycle without mean axial drift. Thus the fixed material abscissa in the question is leading-order notation; this correction does not change the averaged propulsive term below. An imposed mean translation would contribute its separate ordinary axial drag.

To leading nonzero order,

$$
f_x=-\xi_\parallel v_x+C\,y_x y_t,\qquad
-\mathbf f\cdot\mathbf v=\xi_\perp y_t^2+\text{higher-order terms},
\qquad ds=dx+\text{higher-order terms}.
$$

The time-averaged deformation-induced [propulsive force of a periodic planar filament](../../../../../propulsive-force-of-a-periodic-planar-filament.md) and [power of a periodic planar filament](../../../../../power-of-a-periodic-planar-filament.md) are consequently

$$
\boxed{F_x=\frac C T\int_0^T\!\!\int_0^\lambda y_x y_t\,dx\,dt,\qquad
\dot W=\frac{\xi_\perp}{T}\int_0^T\!\!\int_0^\lambda y_t^2\,dx\,dt.}
$$

These are the leading quadratic functionals. Their signs refer to force on the filament. For example, $y=a\sin(kx-\Omega t)$ gives negative $F_x$, opposing the direction of wave propagation.

Let $\eta(x,t)$ be an arbitrary smooth variation periodic in both variables. The [first variation](../../../../../first-variation.md) of the constrained functional is

$$
\delta J=\frac1T\int_0^T\!\!\int_0^\lambda
\left[C(y_t\eta_x+y_x\eta_t)+2\Gamma\xi_\perp y_t\eta_t\right]dx\,dt.
$$

Using [integration by parts](../../../../../integration-by-parts.md) in $x$ and $t$, every boundary term cancels by [periodic boundary conditions](../../../../../periodic-boundary-conditions.md). Therefore

$$
\delta J=-\frac2T\int_0^T\!\!\int_0^\lambda
\left(Cy_{xt}+\Gamma\xi_\perp y_{tt}\right)\eta\,dx\,dt.
$$

The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\boxed{Cy_{xt}+\Gamma\xi_\perp y_{tt}=0.}
$$

For a nontrivial stroke with nonzero thrust, $\Gamma\ne0$. Set $c=C/(\Gamma\xi_\perp)$ and $v=y_t$. Then $v_t+c v_x=0$, whose [method of characteristics](../../../../../method-of-characteristics.md) solution is $v=V(x-ct)$. Integrating in time gives the [travelling-wave stationarity of planar filament propulsion](../../../../../travelling-wave-stationarity-of-planar-filament-propulsion.md):

$$
\boxed{y(x,t)=f(x-ct)+g(x),\qquad
c=\frac{\xi_\perp-\xi_\parallel}{\Gamma\xi_\perp}.}
$$

Here $g$ is an arbitrary static periodic component. It contributes neither power nor mean propulsion because the time average of $y_t$ vanishes. It can be set to zero when describing the active stroke. The wave must be compatible with both specified periods: $f(x-cT)=f(x)$.

For a pure [travelling wave](../../../../../travelling-wave.md), its leading force and power are

$$
F_x=-Cc\int_0^\lambda[f'(x)]^2dx,\qquad
\dot W=\xi_\perp c^2\int_0^\lambda[f'(x)]^2dx,\qquad
\boxed{\frac{F_x}{\dot W}=-\frac{C}{\xi_\perp c}.}
$$

Thus positive $x$ propulsion uses a wave travelling in the negative $x$ direction. Any smooth interior maximizer satisfying only the stated power constraint must have this travelling active deformation. If the drag were isotropic, $C=0$ and there would be no leading propulsion.

There is a qualification to the printed maximization claim: **the variation proves stationarity, not the existence of an unrestricted global maximum**. The [bandwidth limitation in fixed-power filament optimization](../../../../../bandwidth-limitation-in-fixed-power-filament-optimization.md) can be seen directly. Set $k=2\pi/\lambda$, $\Omega=2\pi/T$, and consider $y_m=a\sin(mkx+\Omega t)$. The leading expressions give

$$
\dot W=\frac12\xi_\perp\lambda a^2\Omega^2,\qquad
F_x=\frac12C\lambda a^2mk\Omega.
$$

At fixed power the formal quadratic objective increases with $m$. Eventually that sequence violates the small-slope approximation, but the approximation supplies no numerical slope or wavelength cutoff with which to define the global optimization. Even within a strict small-slope neighbourhood, a sufficiently small admixture of a higher spatial harmonic can improve a candidate interior maximum while keeping power fixed. For example, $y=a[\sqrt{1-\eta^2}\sin(kx+\Omega t)+\eta\sin(mkx+\Omega t)]$ retains the fundamental periods and exactly the same leading power, while its force is multiplied by $1+(m-1)\eta^2$. For fixed $m>1$, taking $a$ and $\eta$ small keeps every slope small.

With an explicit admissible Fourier bandwidth or an additional geometric constraint, the intended conclusion can be made precise. For a finite set of nonstatic [Fourier series](../../../../../fourier-series-split.md) modes proportional to $e^{i(k_jx-\Omega_jt)}$, with wavenumbers $k_j$ and frequencies $\Omega_j$,

$$
\frac{F_x}{\dot W}
=-\frac C{\xi_\perp}
\frac{\sum_j k_j\Omega_j|a_j|^2}
{\sum_j\Omega_j^2|a_j|^2}.
$$

This is a weighted average of $-Ck_j/(\xi_\perp\Omega_j)$. A largest allowed ratio is attained by a single travelling mode, or by modes sharing the same phase speed; their superposition is still a [travelling wave](../../../../../travelling-wave.md). Thus the Euler-Lagrange calculation yields the requested travelling-wave form, while a global maximum requires a specified admissible shape class.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
