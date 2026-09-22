<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [geometrized units](../../../../../geometrized-units.md) $G=c=1$ and [metric signature](../../../../../metric-signature.md) $(-+++)$; $\tau$ is [proper time](../../../../../proper-time.md). The [Killing vectors](../../../../../killing-vector-field.md) $\partial_t$ and $\partial_\phi$ of the [Schwarzschild metric](../../../../../schwarzschild-spacetime.md) give the conserved specific [Killing energy](../../../../../killing-energy.md) and specific [angular momentum](../../../../../angular-momentum.md)

$$
e=\frac Em=\left(1-\frac{2M}{r}\right)\dot t=1,\qquad
h=r^2\dot\phi.
$$

Put $f=1-2M/r$. In the equatorial plane $\dot\theta=0$, and normalization of the [four-velocity](../../../../../four-velocity.md) gives

$$
-1=-f\dot t^2+f^{-1}\dot r^2+r^2\dot\phi^2,
\qquad
\dot r^2=1-f\left(1+\frac{h^2}{r^2}\right)
=\frac{2Mr^2-h^2(r-2M)}{r^3}.
$$

Choosing the inward branch therefore yields

$$
\boxed{u^\mu=\left(\frac r{r-2M},\
-\frac{\sqrt{2Mr^2-h^2(r-2M)}}{r^{3/2}},\
0,\ \frac h{r^2}\right).}
$$

The divergence of the time component at the [Schwarzschild event horizon](../../../../../schwarzschild-event-horizon.md) is a coordinate effect; the inward radial component tends to $-1$.

**Capture from infinity.** To reach the [event horizon](../../../../../event-horizon.md) from infinity, the radial square must remain nonnegative throughout $r>2M$. Equivalently,

$$
h^2\leq\frac{2Mr^2}{r-2M}\quad\text{for all }r>2M.
$$

Differentiating the right side gives $2Mr(r-4M)/(r-2M)^2$, so its minimum occurs at $r=4M$ and equals $16M^2$. Thus

$$
\boxed{|h|\leq4M}
$$

is the necessary capture bound. At equality the radial numerator is $2M(r-4M)^2$. An inward particle arriving from larger radii approaches the unstable orbit $r=4M$ only after infinite [proper time](../../../../../proper-time.md), because $\dot r$ is proportional to $-(r-4M)$ near that orbit. Actual plunges from infinity require $|h|<4M$. This is [Schwarzschild marginally bound capture](../../../../../schwarzschild-marginally-bound-capture.md).

The origin-at-infinity hypothesis is important and is not explicit in the PDF. A particle already inside the angular-momentum barrier can plunge with larger $|h|$. For example, $h=10M$ and initial radius $r_0=2.01M$ give positive radial numerator $7.0802M^3$, remaining positive as $r$ decreases to $2M$. This trajectory has $e=1$ and reaches the [event horizon](../../../../../event-horizon.md). Thus an unrestricted claim about every inward particle would be false; the bound is the intended capture-from-infinity statement.

**Invariant collision energy.** At a collision, the total [four-momentum](../../../../../four-momentum.md) is $P^\mu=m(u_1^\mu+u_2^\mu)$. The invariant [center-of-mass energy](../../../../../center-of-mass-energy.md) uses the covariant metric:

$$
E_{\rm com}^2=-g_{\mu\nu}P^\mu P^\nu.
$$

The PDF instead prints a raised metric multiplying raised velocities. That contraction is not a tensor scalar; the corrected expression above, or a raised metric with lowered momenta, is required. Since each [four-velocity](../../../../../four-velocity.md) has norm $-1$,

$$
\boxed{E_{\rm com}^2=2m^2(1-g_{\mu\nu}u_1^\mu u_2^\nu).}
$$

Let $D_i=2Mr^2-h_i^2(r-2M)$. For two inward trajectories the radial product is positive, and direct substitution into the [Schwarzschild metric](../../../../../schwarzschild-spacetime.md) gives

$$
g_{\mu\nu}u_1^\mu u_2^\nu
=-\frac r{r-2M}
+\frac{\sqrt{D_1D_2}}{r^2(r-2M)}
+\frac{h_1h_2}{r^2}.
$$

Putting these terms over one denominator proves

$$
\boxed{E_{\rm com}^2=
\frac{2m^2}{r^2(r-2M)}
\left[2r^2(r-M)-h_1h_2(r-2M)-\sqrt{D_1D_2}\right].}
$$

**Horizon limit and the upper bound.** A cancellation-free way to take the limit is to write $a_i=1+h_i^2/r^2$ and $\dot r_i=-\sqrt{1-fa_i}$. As $f\to0^+$,

$$
\sqrt{(1-fa_1)(1-fa_2)}
=1-\frac f2(a_1+a_2)+O(f^2).
$$

Hence

$$
1-g(u_1,u_2)
=1+\frac{1-\sqrt{(1-fa_1)(1-fa_2)}}f-\frac{h_1h_2}{r^2}
=2+\frac{(h_1-h_2)^2}{2r^2}+O(f),
$$

and therefore

$$
\boxed{\lim_{r\downarrow2M}E_{\rm com}^2
=m^2\left[4+\frac{(h_1-h_2)^2}{4M^2}\right].}
$$

For particles captured from infinity, $|h_1-h_2|\leq8M$, giving **$E_{\rm com}\leq m\sqrt{20}$** in the horizon limit. For actual captured trajectories the inequality is strict, but the supremum is approached by $h_1\to4M^-$ and $h_2\to-4M^+$. Their azimuthal starting positions can be chosen so that the trajectories meet. If particles may instead be prepared near the [event horizon](../../../../../event-horizon.md), the counterexample $h_1=10M$, $h_2=-10M$ has limiting energy $m\sqrt{104}$; no universal $m\sqrt{20}$ bound then follows.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
