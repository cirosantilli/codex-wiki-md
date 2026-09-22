<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [particle horizon](../../../../../particle-horizon.md) is the greatest distance from which a light signal could have reached the observer since the initial cosmic time $t_i$. Its comoving radius and its radial proper distance at time $t$ are

$$
\chi_h(t)=\int_{t_i}^t\frac{dt'}{a(t')},\qquad
\boxed{d_h(t)=a(t)\int_{t_i}^t\frac{dt'}{a(t')}.}
$$

Here proper distance is measured along the spatial slice, rather than by the transverse area of a sphere. The [Hubble parameter](../../../../../hubble-parameter.md), [deceleration parameter](../../../../../deceleration-parameter.md) and [cosmological density parameter](../../../../../cosmological-density-parameter.md) are

$$
\boxed{H=\frac{\dot a}{a},\qquad q=-\frac{a\ddot a}{\dot a^2},\qquad
\Omega=\frac{\rho}{\rho_{\rm cr}},\qquad\rho_{\rm cr}=\frac{3H^2}{\kappa}.}
$$

The last expression defines the [critical density](../../../../../critical-density.md). For [blackbody radiation](../../../../../black-body-radiation.md), $p=\rho/3$, so the [Friedmann acceleration equation](../../../../../friedmann-acceleration-equation.md) gives $\ddot a/a=-\kappa\rho/3$. Consequently

$$
\boxed{q=\frac{\kappa\rho}{3H^2}=\Omega.}
$$

This is the [radiation relation between deceleration and density](../../../../../radiation-relation-between-deceleration-and-density.md). It does not require spatial flatness.

For the [open radiation universe particle horizon](../../../../../open-radiation-universe-particle-horizon.md), write $x=a/a_0$. The [cosmological continuity equation](../../../../../cosmological-continuity-equation.md) gives $\rho=\rho_0x^{-4}$, while the present [Friedmann equation](../../../../../friedmann-equations.md) gives $-k/a_0^2=H_0^2(1-\Omega_0)$. Thus

$$
H^2=H_0^2\left[\Omega_0x^{-4}+(1-\Omega_0)x^{-2}\right],\qquad
\dot x=\frac{H_0}{x}\sqrt{\Omega_0+(1-\Omega_0)x^2}.
$$

Taking the big-bang endpoint $x=0$ and using $dt=dx/\dot x$, the present radial proper distance becomes

$$
\begin{aligned}
d_{h0}&=\int_0^1\frac{dx}{x\dot x}
=\frac1{H_0}\int_0^1\frac{dx}{\sqrt{\Omega_0+(1-\Omega_0)x^2}}\\
&=\frac{\operatorname{arsinh}\sqrt{(1-\Omega_0)/\Omega_0}}
{H_0\sqrt{1-\Omega_0}}.
\end{aligned}
$$

Therefore

$$
\boxed{d_{h0}=\frac1{H_0\sqrt{1-\Omega_0}}
\ln\left[\sqrt{\frac{1-\Omega_0}{\Omega_0}}+
\sqrt{1+\frac{1-\Omega_0}{\Omega_0}}\right].}
$$

The formula applies to $0<\Omega_0<1$. Its flat-radiation limit is $H_0d_{h0}\to1$, agreeing with $a\propto t^{1/2}$ and $d_h=2t=H^{-1}$. The divergence as $\Omega_0\to0$ reflects the unbounded past conformal interval of the limiting empty open model; that endpoint is not a radiation-filled universe.

The [horizon problem](../../../../../horizon-problem.md) concerns the nearly uniform temperature of widely separated parts of the [cosmic microwave background](../../../../../cosmic-microwave-background.md). In a purely decelerating [Hot Big Bang model](../../../../../hot-big-bang-model.md), their past light cones at last scattering do not overlap far enough to explain this agreement by thermal contact. During [cosmic inflation](../../../../../cosmic-inflation-split.md), accelerated expansion shrinks the [comoving Hubble radius](../../../../../comoving-hubble-radius.md). A patch initially small enough for causal communication can be stretched to encompass the later observable universe. [Reheating](../../../../../reheating.md) converts the inflationary energy into a hot plasma with correlated initial conditions across that patch. Enough inflation must occur before the observable scales leave the [Hubble radius](../../../../../hubble-radius.md); inflation cannot establish contact between regions that were never initially causally related.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
