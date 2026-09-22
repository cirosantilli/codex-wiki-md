<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Effective [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md).** Work to leading order in the slender-layer ratio $H/L$. Take the growing lower wedge to have [porous permeability](../../../../../permeability-of-a-porous-medium.md) $k_1$, with interface $y=Hx/L$, and the upper wedge to have [porous permeability](../../../../../permeability-of-a-porous-medium.md) $k_2$. The leading [pressure](../../../../../pressure.md) is independent of $y$; vertical flow is smaller than horizontal flow by $H/L$. Define

$$
\xi=\frac{x}{L},\qquad K(\xi)=k_2+(k_1-k_2)\xi.
$$

[Darcy's law](../../../../../darcy-law.md) and the fixed two-dimensional [volume flux](../../../../../volumetric-flow-rate.md) give

$$
Q=-\frac{H K(\xi)}{\mu}p_x,\qquad
q_i(x)=\frac{Qk_i}{HK(\xi)}.
$$

Here $q_i$ is [Darcy velocity](../../../../../darcy-velocity.md); the parcel speed is $q_i/\phi$. Integrating the [pressure gradient](../../../../../pressure-gradient.md) over the length and defining $Q=Hk_{\rm eff}\Delta p/(\mu L)$ yields

$$
\boxed{k_{\rm eff}=\frac{k_1-k_2}{\log(k_1/k_2)}.}
$$

The equal-[porous permeability](../../../../../permeability-of-a-porous-medium.md) limit is $k_{\rm eff}=k_1=k_2$. This logarithmic mean comes from parallel layers at each cross-section followed by series addition of their local hydraulic resistances. It is a slender-layer result; a full two-dimensional transmission problem has small end and interface corrections.

**Parcel paths and travel times.** Pressure equalization does not mean that parcels stay at fixed $y$: [mass conservation](../../../../../mass-conservation.md) requires a small vertical flow. Define a [streamfunction](../../../../../stream-function.md) by $\psi(x,0)=0$ and $\psi(x,H)=Q$. Its leading expression is

$$
\psi=\begin{cases}q_1(x)y,&y\leq H\xi,\\Q-q_2(x)(H-y),&y\geq H\xi.\end{cases}
$$

Let $r=y_0/H$ label a parcel released at the inlet. There $\psi=Qr$. At the inclined interface $\psi/Q=k_1\xi/K(\xi)$, so the parcel crosses from the upper wedge into the lower one at

$$
\boxed{\xi_c(r)=\frac{rk_2}{k_1(1-r)+k_2r}.}
$$

Before crossing, $y/H=1-(1-r)K/k_2$; afterwards, $y/H=rK/k_1$. These expressions show why integrating the speed along a horizontal line would give the wrong parcel time.

Put $d=k_1-k_2$ and $\tau_V=\phi HL/Q$, the pore-volume throughput time. Integrating $dt=\phi\,dx/q_i$ on the two portions of the path gives

$$
\boxed{\begin{aligned}
\tau(y_0)&=\tau_V\left[\frac1{k_2}\int_0^{\xi_c}K(\xi)d\xi
+\frac1{k_1}\int_{\xi_c}^{1}K(\xi)d\xi\right]\\
&=\tau_V\left[\frac{k_1+k_2}{2k_1}
+\frac d{k_1}\xi_c+\frac{d^2}{2k_1k_2}\xi_c^2\right].
\end{aligned}}
$$

Its derivative with respect to $\xi_c$ is $\tau_V dK/(k_1k_2)$, so it is monotone. The limiting streamline times at the lower and upper boundaries are $\tau_V(k_1+k_2)/(2k_1)$ and $\tau_V(k_1+k_2)/(2k_2)$ respectively. Hence

$$
\boxed{\Delta\tau_{\max}=\frac{\phi HL}{2Q}
\frac{|k_1^2-k_2^2|}{k_1k_2}.}
$$

The printed expression assumes $k_1\geq k_2$. The absolute value is needed for a nonnegative maximum difference without that ordering. For equal [porous permeabilities](../../../../../permeability-of-a-porous-medium.md) every parcel has time $\tau_V$.

<a id="1/image-streamlines-crossing-an-inclined-permeability-interface-in-a-slender-layer-with-lower-wedge-permeability-ten-times-the-upper-wedge-permeability"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-78-layered-streamlines.png)

**[Figure 1](#1/image-streamlines-crossing-an-inclined-permeability-interface-in-a-slender-layer-with-lower-wedge-permeability-ten-times-the-upper-wedge-permeability). Streamlines crossing an inclined permeability interface in a slender layer with lower-wedge permeability ten times the upper-wedge permeability**.

**Oil recovery.** In the ideal passive-displacement model with $k_1/k_2=10$, the earliest and latest travel times are $0.55\tau_V$ and $5.5\tau_V$, a spread of $4.95\tau_V$. Preferential paths through the high-[porous permeability](../../../../../permeability-of-a-porous-medium.md) wedge therefore give early water breakthrough while oil on slower paths remains unswept. Continued injection sends much water through paths already swept; complete displacement requires several pore volumes. The [flux-weighted residence time in a porous layer](../../../../../flux-weighted-residence-time-in-a-porous-layer.md) remains $\tau_V$. Real [waterflooding](../../../../../waterflooding.md) also depends on [phase mobilities](../../../../../phase-mobility.md), [relative permeabilities](../../../../../relative-permeability.md), [capillary pressure](../../../../../capillary-pressure.md) and mixing, so these numbers illustrate heterogeneity rather than a quantitative two-phase recovery prediction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
