<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the secular, circular-orbit approximation: the wind escapes fast enough to avoid appreciable interaction with the companion, while the stellar masses change slowly enough that orbital elements describe the evolving [binary star](../../../../../binary-star.md). Neglect spin [angular momentum](../../../../../angular-momentum.md). Let $\omega=(GM/a^3)^{1/2}$ be the orbital angular speed. The donor's distance from the centre of mass is $a_1=aM_2/M$, and the [circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md) is

$$
J_{\rm orb}=\frac{M_1M_2}{M}a^2\omega=M_1M_2\left(\frac{Ga}{M}\right)^{1/2}.
$$

A spherically symmetric wind in the donor frame has zero mean additional angular momentum about the donor. Averaging its angular momentum about the binary centre of mass therefore gives the donor's orbital specific angular momentum, $j_1=a_1^2\omega$. Since $\dot M<0$ denotes mass removed from the system, $\dot J_{\rm orb}=j_1\dot M$, and

$$
\boxed{\frac{\dot J_{\rm orb}}{J_{\rm orb}}=\frac{M_2\dot M}{M_1M}}.
$$

This is [donor-wind angular-momentum loss](../../../../../donor-wind-angular-momentum-loss.md) in the [Jeans-mode mass loss](../../../../../jeans-mode-mass-loss.md) approximation.

First allow only wind loss, so $\dot M_1=\dot M$ and $\dot M_2=0$. The logarithmic derivative of $J_{\rm orb}$ gives

$$
\frac{M_2\dot M}{M_1M}=\frac{\dot M}{M_1}+\frac12\frac{\dot a}{a}-\frac12\frac{\dot M}{M}.
$$

Solving yields $\dot a/a=-\dot M/M$. By [Kepler's third law](../../../../../kepler-s-third-law.md), $P^2=4\pi^2a^3/(GM)$, so $\dot P/P=-2\dot M/M$. Integrating gives

$$
\boxed{aM=\mathrm{constant},\qquad PM^2=\mathrm{constant}}.
$$

Wind loss thus expands the separation and lengthens the orbital period. These are secular relations; an impulsive loss on an orbital time could instead generate eccentricity and would need a different analysis.

To test contact, put $D=d\log(R_1/R_L)/dt$. The given short-time [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md) gives $\dot R_1/R_1=-n\dot M_1/M_1$. Differentiating the [Roche lobe](../../../../../roche-lobe.md) approximation gives

$$
\frac{\dot R_L}{R_L}=\frac{\dot a}{a}+\frac13\left(\frac{\dot M_1}{M_1}-\frac{\dot M}{M}\right).
$$

For wind alone this becomes $\dot R_L/R_L=\dot M/(3M_1)-4\dot M/(3M)$. Hence, with the [binary mass ratio](../../../../../binary-mass-ratio.md) $q=M_1/M_2$,

$$
D_{\rm w}=-\left(n+\frac13\right)\frac{\dot M}{M_1}+\frac{4\dot M}{3M}=\frac{\dot M}{3M_1(1+q)}\left[3(1-n)q-(1+3n)\right].
$$

Because $\dot M$ is negative, increasing overfill, $D_{\rm w}>0$, occurs precisely when

$$
\boxed{q<\frac{1+3n}{3(1-n)}}.
$$

This is [wind-driven Roche-lobe overflow](../../../../../wind-driven-roche-lobe-overflow.md). For the reverse strict inequality, $D_{\rm w}<0$ and the [donor star](../../../../../donor-star.md) retreats inside its [Roche lobe](../../../../../roche-lobe.md), producing a [detached binary](../../../../../detached-binary.md). At equality the wind is neutral to contact at this order.

Now permit an additional [conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md) rate $x=\dot M_2$ to the [mass-gaining star](../../../../../mass-gaining-star.md). The total escaping wind remains $\dot M$, while $\dot M_1=\dot M-x$. Transfer retains orbital angular momentum within the binary under the assumed neglect of spins, so the same wind-loss formula for $\dot J_{\rm orb}$ applies. Logarithmic differentiation now gives

$$
\frac{\dot a}{a}=-\frac{\dot M}{M}+2x\left(\frac1{M_1}-\frac1{M_2}\right).
$$

Substituting this and $\dot M_1=\dot M-x$ into the two radius derivatives gives

$$
D=D_{\rm w}+\frac{x}{3M_1}(6q-5+3n).
$$

Steady contact requires $D=0$. If the wind is driving overflow and $6q<5-3n$, the transfer contribution reduces overfill and a positive contact rate exists:

$$
\boxed{\dot M_2=-\frac{1+3n-3(1-n)q}{(1+q)(5-3n-6q)}\dot M}.
$$

The numerator and denominator are positive in this regime, making $\dot M_2>0$. This explicitly establishes both the [contact transfer rate with Jeans-mode wind loss](../../../../../contact-transfer-rate-with-jeans-mode-wind-loss.md) and its stabilizing sign.

If the wind drives overflow but $6q>5-3n$, positive transfer instead increases $R_1/R_L$: the mass loss required to relieve overfill makes the overfill worse. The formal contact formula would require $\dot M_2<0$, which is not donor-to-companion transfer. **There is no stabilizing positive contact rate; overflow runs away.** For a [red giant](../../../../../red-giant.md) this can lead to a [common envelope](../../../../../common-envelope.md), followed by envelope ejection into a tighter binary or a merger. The criterion concerns the supplied short-time radius response; the actual runaway timescale and outcome require the donor's dynamical and thermal response. At $6q=5-3n$ transfer is neutral to contact at this order, so it cannot balance a nonzero wind driver. If the wind already causes detachment, the transfer instability condition alone does not initiate overflow.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
