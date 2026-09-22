<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Orbital [angular momentum](../../../../../angular-momentum.md) carried by the wind.** Use a circular orbit of separation $a$, and write $M=M_1+M_2$ and $\Omega_o^2=GM/a^3$. The donor's distance from the center of mass is $a_1=aM_2/M$. With spins neglected, its specific orbital [angular momentum](../../../../../angular-momentum.md) is $j_1=a_1^2\Omega_o$, while the [circular-binary orbital angular momentum](../../../../../circular-binary-orbital-angular-momentum.md) is

$$
J_{\rm orb}=\frac{M_1M_2}{M}a^2\Omega_o=M_1M_2\sqrt{\frac{Ga}{M}}.
$$

A fast spherically symmetric [stellar wind](../../../../../stellar-wind.md) has no net extra [angular momentum](../../../../../angular-momentum.md) in the donor's rest frame and escapes with mean specific orbital [angular momentum](../../../../../angular-momentum.md) $j_1$. Thus [Jeans-mode mass loss](../../../../../jeans-mode-mass-loss.md) gives

$$
\boxed{\frac{\dot J_{\rm orb}}{J_{\rm orb}}=\frac{j_1\dot M}{J_{\rm orb}}=\frac{M_2\dot M}{M_1M}.}
$$

Initially take negligible wind capture by the companion, so $\dot M_1=\dot M$, $\dot M_2=0$ and the total mass derivative is $\dot M$. Logarithmic differentiation of $J_{\rm orb}$ gives

$$
\frac{\dot J_{\rm orb}}{J_{\rm orb}}=\frac{\dot M}{M_1}+\frac12\frac{\dot a}{a}-\frac12\frac{\dot M}{M}.
$$

Combining the two expressions yields $\dot a/a=-\dot M/M$, so $aM$ is constant. [Kepler's third law](../../../../../kepler-s-third-law.md) then gives $\dot P/P=(3/2)\dot a/a-(1/2)\dot M/M=-2\dot M/M$. Hence

$$
\boxed{a\propto M^{-1},\qquad P\propto M^{-2}.}
$$

These are secular relations for slow changes of the orbit through nearly circular states. A wind being fast compared with orbital speed does not mean its mass-loss timescale is shorter than an orbital period; impulsive removal would require a different orbital calculation.

**Whether wind drives contact.** Ignore nuclear expansion on the stated short evolutionary timescale. With $R_1\propto M_1^{-n}$ and $R_L\propto a(M_1/M)^{1/3}$, wind alone gives

$$
\begin{aligned}
\frac{d}{dt}\ln\frac{R_1}{R_L}
&=-\left(n+\frac13\right)\frac{\dot M}{M_1}+\frac43\frac{\dot M}{M}\\
&=\frac{\dot M}{3M_1(1+q)}[3(1-n)q-(1+3n)],\qquad q=\frac{M_1}{M_2}.
\end{aligned}
$$

Because $\dot M<0$, the ratio increases precisely when

$$
\boxed{q<\frac{1+3n}{3(1-n)}.}
$$

This is [wind-driven Roche-lobe overflow](../../../../../wind-driven-roche-lobe-overflow.md): the escaping wind makes the donor expand relative to its lobe and drives a separate transfer stream. It is not the slow-wind capture mechanism called [Wind Roche-lobe overflow](../../../../../wind-roche-lobe-overflow.md). If the inequality is reversed, the donor recedes inside its expanding lobe and detaches; wind loss alone does not maintain a Roche-lobe transfer stream. At equality it gives no leading-order change of overfill, so additional evolution or higher-order changes decide the outcome.

**Contact rate and its stability.** Now let the transfer stream be accreted conservatively by star 2 while the separate wind still escapes at rate $\dot M<0$. Denote the stream rate by $\dot M_2>0$. Then

$$
\dot M_1=\dot M-\dot M_2,\qquad\dot M_{\rm total}=\dot M.
$$

Only the wind removes orbital [angular momentum](../../../../../angular-momentum.md); internal transfer redistributes it. Using the same wind-loss law and differentiating $J_{\rm orb}$ gives

$$
\frac{\dot a}{a}=-\frac{\dot M}{M}+2\dot M_2\left(\frac1{M_1}-\frac1{M_2}\right).
$$

Substitute this into the donor and lobe radius derivatives. The overfill evolves as

$$
\frac{d}{dt}\ln\frac{R_1}{R_L}
=-\frac{\dot M}{3M_1(1+q)}[1+3n-3(1-n)q]
-\frac{\dot M_2}{3M_1}[5-3n-6q].
$$

Maintaining contact sets the left side to zero and gives the [contact transfer rate with Jeans-mode wind loss](../../../../../contact-transfer-rate-with-jeans-mode-wind-loss.md),

$$
\boxed{\dot M_2=-\frac{1+3n-3(1-n)q}{(1+q)(5-3n-6q)}\dot M.}
$$

When the wind-drive condition holds, its numerator is positive. If $6q<5-3n$, the denominator is also positive and the stream rate is positive; increasing transfer reduces overfill and can balance the wind driver.

If instead $6q>5-3n$, positive transfer increases overfill, which drives still more transfer. The formal contact formula would demand a negative stream rate and is not a physical steady solution. **The system develops unstable, runaway mass transfer** on the timescale appropriate to the assumed donor response. For a giant with an adiabatically responding envelope, this can lead to a [common envelope](../../../../../common-envelope.md) and rapid orbital evolution, rather than the stable contact sequence; the eventual outcome requires physics beyond these radius laws. At $6q=5-3n$, transfer gives no linear restoring effect, and a nonzero wind driver cannot be balanced by a finite rate within this approximation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
