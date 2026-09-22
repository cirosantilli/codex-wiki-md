<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For [Roche-lobe overflow](../../../../../roche-lobe-overflow.md), $R_2=R_L$. Cubing the [Roche lobe](../../../../../roche-lobe.md) approximation and using the donor's [mass-radius relation](../../../../../mass-radius-relation.md) gives

$$
a^3=\frac{R_2^3}{0.46^3}\frac M{M_2}=\frac{R_\odot^3}{0.46^3}\frac{M M_2^2}{M_\odot^3}.
$$

[Kepler's third law](../../../../../kepler-s-third-law.md) therefore yields the [Roche-lobe period-mass relation for a linear donor radius law](../../../../../roche-lobe-period-mass-relation-for-a-linear-donor-radius-law.md):

$$
\boxed{\frac P{P_0}=\frac{M_2}{M_\odot}},\qquad P_0=2\pi\sqrt{\frac{R_\odot^3}{0.46^3GM_\odot}}.
$$

The component distances from the [centre of mass](../../../../../center-of-mass.md) are $a_1=aM_2/M$ and $a_2=aM_1/M$. Summing their [angular momenta](../../../../../angular-momentum.md) gives the [circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md)

$$
\boxed{J=(M_1a_1^2+M_2a_2^2)\Omega=\frac{M_1M_2}{M}a^2\Omega=M_1M_2\sqrt{\frac{Ga}{M}}}.
$$

During [conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md), $\dot M=0$ and $\dot M_1=-\dot M_2$. Logarithmic differentiation at constant [angular momentum](../../../../../angular-momentum.md) gives $\dot a/a=-2(1-q)\dot M_2/M_2$. Thus the [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) gives

$$
\boxed{\frac{\dot R_L}{R_L}=\left(2q-\frac53\right)\frac{\dot M_2}{M_2}},\qquad \frac{\dot R_2}{R_2}=\frac{\dot M_2}{M_2}.
$$

Their difference is $d\log(R_L/R_2)/dt=(2q-8/3)\dot M_2/M_2$. Since the donor loses [mass](../../../../../mass.md), this is positive for $q<4/3$: **the donor shrinks relative to its Roche lobe, so transfer shuts off without an external driver.** The [Roche lobe](../../../../../roche-lobe.md) itself expands only for $q<5/6$; for $5/6<q<4/3$ it shrinks more slowly than the donor.

[Gravitational-wave emission from a binary system](../../../../../gravitational-wave-emission-from-a-binary-system.md) provides such a driver: the orbit emits [gravitational waves](../../../../../gravitational-wave.md) carrying [energy](../../../../../energy.md) and [angular momentum](../../../../../angular-momentum.md), and the shrinking [Roche lobe](../../../../../roche-lobe.md) can maintain contact. Allowing $\dot J<0$, the [binary mass-transfer contact equation](../../../../../binary-mass-transfer-contact-equation.md) becomes

$$
\frac{\dot R_L}{R_L}=2\frac{\dot J}{J}+\left(2q-\frac53\right)\frac{\dot M_2}{M_2}=\frac{\dot M_2}{M_2},\qquad \boxed{\frac{\dot M_2}{M_2}=\frac{3}{4-3q}\frac{\dot J}{J}}.
$$

It gives a negative transfer rate for $q<4/3$.

For the [classical nova](../../../../../classical-nova.md), assume [isotropic re-emission from a binary star](../../../../../isotropic-re-emission-from-a-binary-star.md): ejecta carry the accretor's [specific angular momentum](../../../../../specific-angular-momentum.md) $j_1=a_1^2\Omega$. The eruption lasts many [orbital periods](../../../../../orbital-period.md), so the orbit responds approximately adiabatically and remains nearly circular; an instantaneous asymmetric kick would be a different model. To first order,

$$
\frac{\delta J}{J}=-\frac{j_1\delta m}{J}=-q\frac{\delta m}{M},\qquad \delta M_1=-\delta m,\qquad\delta M_2=0,\qquad\delta M=-\delta m.
$$

Differentiating the [circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md) formula during the ejection gives

$$
-q\frac{\delta m}{M}=-\frac{\delta m}{M_1}+\frac12\frac{\delta a}{a}+\frac12\frac{\delta m}{M},\qquad \boxed{\frac{\delta a}{a}=\frac{\delta m}{M}}.
$$

The accompanying [Roche lobe](../../../../../roche-lobe.md) change is therefore

$$
\boxed{\frac{\delta R_L}{R_L}=\frac{\delta a}{a}+\frac13\frac{\delta m}{M}=\frac{4\delta m}{3M}}.
$$

The donor does not change [mass](../../../../../mass.md) in the eruption and moves inside its expanded [Roche lobe](../../../../../roche-lobe.md): this is [nova-induced binary detachment](../../../../../nova-induced-binary-detachment.md).

Put $\Gamma=-\dot J>0$ for the constant external loss. During detachment the component masses are fixed, so the [Roche lobe](../../../../../roche-lobe.md) shrinks at fractional rate $2\Gamma/J$. Closing the fractional gap $4\delta m/(3M)$ takes $t_d=2J\delta m/(3M\Gamma)$. During the subsequent [semidetached binary](../../../../../semidetached-binary.md) phase, the [binary mass-transfer contact equation](../../../../../binary-mass-transfer-contact-equation.md) gives $|\dot M_2|=3M_2\Gamma/[J(4-3q)]$, so accumulating the next eruption's [mass](../../../../../mass.md) takes $t_s=J(4-3q)\delta m/(3M_2\Gamma)$. Consequently

$$
\boxed{\frac{t_d}{t_s}=\frac{2M_2}{M(4-3q)}=\frac{2q}{(4-3q)(1+q)}}.
$$

Both times are evaluated to first order in $\delta m/M$, with the same equilibrium donor [mass-radius relation](../../../../../mass-radius-relation.md); changes of $q,J$ and the transfer rate within one cycle affect higher orders.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
