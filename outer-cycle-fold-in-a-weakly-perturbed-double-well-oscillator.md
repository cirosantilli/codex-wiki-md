# Outer-cycle fold in a weakly perturbed double-well oscillator

↑ **Parent:** [Energy balance for the weakly perturbed double-well oscillator](energy-balance-for-the-weakly-perturbed-double-well-oscillator.md)

For $u'=v$, $v'=u-u^3+\varepsilon(\beta-u^2)v$, let $H=v^2/2-u^2/2+u^4/4$. On an outer [periodic orbit](periodic-orbit.md) with $H>0$, leading [energy balance method](energy-balance-method.md) requires $\beta=B(H)$, where

$$
B(H)=\frac{\int_0^{u_{\max}(H)}u^2\sqrt{2H+u^2-u^4/2}\,du}{\int_0^{u_{\max}(H)}\sqrt{2H+u^2-u^4/2}\,du}.
$$

Here $u_{\max}^2=1+\sqrt{1+4H}$. The [homoclinic orbit](homoclinic-orbit.md) limit is $B(0)=4/5$. Differentiating the denominator gives a period integral diverging at $H=0$, whereas the derivative of the numerator stays finite; hence $B$ decreases immediately above zero. At large $H$, rescaling $u=H^{1/4}s$ gives $B(H)\propto\sqrt H$. Its first nondegenerate minimum selects a [saddle-node bifurcation of periodic orbits](saddle-node-bifurcation-of-periodic-orbits.md); numerical quadrature gives $\beta_{\rm fold}\simeq0.75226$. The cycle on the decreasing portion is unstable and the one on the increasing portion is stable, since the net energy drift has sign $\beta-B(H)$. Restoring an unperturbed coefficient $a^2$ in the linear restoring term multiplies the threshold by $a^2$.

## ↑ Ancestors (6)

1. [Energy balance for the weakly perturbed double-well oscillator](energy-balance-for-the-weakly-perturbed-double-well-oscillator.md)
2. [Energy balance method](energy-balance-method.md)
3. [Dynamical systems](dynamical-systems-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-56/1/d/solution.md)
