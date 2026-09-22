<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume well-mixed populations, exponential prey growth without density regulation, predator mortality without food, and bilinear encounters. The [Lotka-Volterra predator-prey model](../../../../../lotka-volterra-predator-prey-model.md) is

$$
\dot X=X(a-bY),\qquad \dot Y=Y(cX-d),\qquad a,b,c,d>0.
$$

Its coexistence [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is $X_*=d/c$, $Y_*=a/b$. The [Jacobian matrix](../../../../../jacobian-matrix.md) there has [eigenvalues](../../../../../eigenvalue.md) $\pm i\sqrt{ad}$, so it is a [center equilibrium](../../../../../center-equilibrium.md) rather than an attracting [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md). More globally,

$$
H(X,Y)=cX-d\log X+bY-a\log Y
$$

is a [first integral](../../../../../first-integral.md): substituting the two equations into $\dot H$ gives zero. It has a strict minimum at coexistence, diverges at the boundary and at infinity, and its other positive-quadrant level sets are closed [periodic orbits](../../../../../periodic-orbit.md). Small oscillations have frequency $\omega=\sqrt{ad}$. In scaled variables $U=\sqrt d(X-X_*)/X_*$ and $V=\sqrt a(Y-Y_*)/Y_*$, the [linearization](../../../../../linearization.md) is $\dot U=-\omega V$, $\dot V=\omega U$.

Model an annual fixed quota as a pulse removing $h>0$ prey, $X^+=X^--h$, $Y^+=Y^-$, with $h<X^-$. Between pulses the original equations apply. In logarithmic coordinates the flow has zero divergence, but the pulse has [determinant](../../../../../determinant.md) $X^-/(X^--h)>1$. Therefore a periodic annually harvested trajectory has [return map](../../../../../poincare-map.md) [determinant](../../../../../determinant.md) greater than one, and cannot have both multipliers inside the unit circle. It is unstable, even when a leading rotation-plus-translation approximation looks neutral. Near a nonresonant small-quota forced orbit this expansion destabilizes the original [center equilibrium](../../../../../center-equilibrium.md); resonant pulse timing can add secular effects. Quotas larger than the remaining prey are not biologically realizable and require stopping the model. This is [fixed-quota harvesting of Lotka-Volterra populations](../../../../../fixed-quota-harvesting-of-lotka-volterra-populations.md).

The common continuous approximation to an annual quota gives $\dot X=X(a-bY)-h$. Its positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is $X_*=d/c$, $Y_h=(a-h/X_*)/b$, requiring $h<aX_*$. Its [Jacobian matrix](../../../../../jacobian-matrix.md) has [trace](../../../../../matrix-trace.md) $h/X_*>0$ and [determinant](../../../../../determinant.md) $bcX_*Y_h>0$, so this approximation also destabilizes coexistence. At small $h$ it is an unstable [focus](../../../../../focus-dynamical-systems.md). A quota is a larger per-capita mortality when prey are scarce, which is the adverse feedback responsible for the result.

For abundance-triggered pulses, retain the same fixed prey removal and specify the crossing direction. The exact [event-triggered harvesting by conserved energy](../../../../../event-triggered-harvesting-by-conserved-energy.md) calculation is

$$
\Delta H=-ch-d\log(1-h/X).
$$

If prey abundance triggers the event at $X=X_c$, this increment is the same at every event. A sufficiently high prey threshold with a modest quota gives $\Delta H<0$: the orbit's oscillation energy decreases until it no longer crosses the threshold, after which harvesting stops. If $X_c\leq X_*$, then $\Delta H>0$ and harvesting increases oscillations. At the balanced threshold satisfying $ch=d\log[X_c/(X_c-h)]$, energy is unchanged and the ideal orbit is neutral. Thus the useful rule is harvesting at high prey abundance, not simply using any fixed threshold; the equality case supplies no asymptotic restoration.

A predator threshold $Y=Y_c$ does not hold prey abundance fixed. On a rising-predator crossing, $X>X_*$, so a sufficiently small harvest initially lowers $H$; on a falling-predator crossing $X<X_*$, it raises $H$. Nevertheless the rising-predator rule is not a robust stabilizer in this conservative model. Its balanced return orbit has preharvest prey abundance

$$
X_h=\frac{h}{1-e^{-h/X_*}},\qquad X_h-h<X_*<X_h,
$$

obtained by equating $cX-d\log X$ before and after the pulse. On the return section the derivative is

$$
\frac{dX_{\rm next}}{dX}\bigg|_{X_h}
=\frac{c-d/(X_h-h)}{c-d/X_h}
=-\frac{e^z-1-z}{z-1+e^{-z}},\qquad z=h/X_*.
$$

Its magnitude exceeds one because $e^z-e^{-z}>2z$ for $z>0$. The balanced predator-triggered cycle is consequently unstable. At leading small-oscillation order its multiplier is $-1$, explaining a marginal alternation rather than stable damping. If the trigger is crossed in both directions, or a variable rather than fixed quota is used, a different return rule results and must be analyzed separately.

For conservation, the ideal model shows why fixed removals can be dangerous and why prey-based high-abundance feedback can be safer than a calendar quota or an unspecified predator threshold. These conclusions depend on the chosen pulse rule and on the absence of density dependence, refuges and stochasticity. They do not justify a universal numerical safe quota. **A harvest policy needs a stopping threshold and the correct phase-dependent feedback, not merely a small nominal annual catch.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
