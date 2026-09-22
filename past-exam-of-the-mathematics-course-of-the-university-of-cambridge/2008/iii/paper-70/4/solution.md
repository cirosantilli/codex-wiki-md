<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $M=M_1+M_2$. In a [circular orbit](../../../../../circular-orbit.md), the distances from the centre of mass are $r_1=aM_2/M$ and $r_2=aM_1/M$. Summing the components' [angular momentum](../../../../../angular-momentum.md) gives

$$
J=(M_1r_1^2+M_2r_2^2)\Omega
=\frac{M_1M_2}{M}a^2\Omega.
$$

Use [Kepler's third law](../../../../../kepler-s-third-law.md) $\Omega^2a^3=GM$ and $\Omega=2\pi/P_{\rm orb}$ to obtain the [circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md)

$$
\boxed{J=\frac{G^{2/3}P_{\rm orb}^{1/3}M_1M_2}
{(2\pi)^{1/3}M^{1/3}}.}
$$

The numerator contains orbital period, not the erroneous $M_{\rm orb}$ token in the converted TeX.

The total mass changes as $\dot M=(1-f)\dot M_1$. With the prescribed wind carrying specific angular momentum $\lambda J/M$, the angular-momentum loss law is $\dot J/J=\lambda\dot M/M$. For constant $\lambda$, integration gives $J\propto M^\lambda$. Cubing the orbital formula then proves the [binary period invariant for a constant wind angular-momentum factor](../../../../../binary-period-invariant-for-a-constant-wind-angular-momentum-factor.md):

$$
\boxed{P_{\rm orb}\propto M_1^{-3}M_2^{-3}M^\delta,
\qquad\delta=3\lambda+1.}
$$

This integration does not require $f$ to be constant, although its instantaneous value enters the following response coefficients. In the conservative case $f=1$, both $M$ and $J$ are constant and the usual [period-product invariant for conservative mass transfer](../../../../../period-product-invariant-for-conservative-mass-transfer.md) is recovered.

Kepler's law and the given [Roche lobe](../../../../../roche-lobe.md) approximation imply $R_L\propto M_1^{1/3}P_{\rm orb}^{2/3}$, since the total-mass factor cancels. Using the period law therefore gives

$$
\log R_L=-\frac53\log M_1-2\log M_2+\frac{2\delta}{3}\log M+\mathrm{constant}.
$$

Because $\dot M_2=-f\dot M_1$, the instantaneous [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) is

$$
\zeta_L=\frac{d\log R_L}{d\log M_1}
=-\frac53+2fq+\frac{2\delta(1-f)q}{3(1+q)},
\qquad q=\frac{M_1}{M_2}.
$$

For $x=\log(R/R_L)$, subtracting this response from the prescribed stellar radius evolution gives

$$
\dot x=\frac1{t_{\rm nuc}}+(n-\zeta_L)\frac{\dot M_1}{M_1}.
$$

The overflow-rate model requires $f>0$ and is used for small positive overfill. It gives $\dot M_1/M_1=-x/(ft_{\rm dyn})$. Hence the [nuclear-driven Roche-overfill relaxation](../../../../../nuclear-driven-roche-overfill-relaxation.md) equation is

$$
\boxed{\dot x=\frac1{t_{\rm nuc}}-\frac{x}{ft_{\rm dyn}}
\left[n+\frac53-2fq-\frac{2\delta(1-f)q}{3(1+q)}\right].}
$$

Let the bracket be $A(q)$. On the short response time, freeze the slowly changing masses and coefficients. If $A>0$, the local solution is

$$
x(t)=x_*+[x(0)-x_*]e^{-At/(ft_{\rm dyn})},\qquad
x_* =\frac{ft_{\rm dyn}}{At_{\rm nuc}}.
$$

The equilibrium donor mass-loss rate is $\dot M_1/M_1=-1/(At_{\rm nuc})$. Thus the required stabilizing mass-ratio condition is

$$
\boxed{n+\frac53>2fq+\frac{2(3\lambda+1)(1-f)q}{3(1+q)}.}
$$

When $A$ is of order one and $t_{\rm dyn}\ll t_{\rm nuc}$, the overfill is small and relaxation is fast, while mass transfer proceeds on a nuclear timescale. A positive $A$ arbitrarily close to zero does not by itself ensure this timescale separation or small overfill.

For an explicit threshold put $B=n+5/3$ and $C_w=2\delta(1-f)/3$. The inequality is

$$
B+(B-2f-C_w)q-2fq^2>0.
$$

If $B>0$ and $f>0$, its positive root gives

$$
\boxed{0<q<q_{\rm crit},\qquad
q_{\rm crit}=\frac{B-2f-C_w+\sqrt{(B-2f-C_w)^2+8fB}}{4f}.}
$$

For $f=1$ this reduces to $q<(n+5/3)/2$, the [conservative mass-transfer critical mass ratio](../../../../../conservative-mass-transfer-critical-mass-ratio.md). For other parameter signs the unsimplified inequality is the general condition.

If $A<0$, a larger overfill causes further growth rather than restoration, on the short scale $ft_{\rm dyn}/|A|$. Transfer runs away towards a dynamical episode, potentially a [common envelope](../../../../../common-envelope.md) or merger; the small-overfill model then fails. At $A=0$ the overfill grows linearly under nuclear expansion and there is no steady regulated contact. These conclusions use the stipulated donor-radius response; an actual dynamical episode requires its adiabatic response and hydrodynamics.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
