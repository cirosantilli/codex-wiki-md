<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a circular binary with negligible spin, the two orbital radii about the center of mass are $a_1=aM_2/M$ and $a_2=aM_1/M$. Summing their orbital [angular momenta](../../../../../angular-momentum.md) gives

$$
\boxed{J=\Omega(M_1a_1^2+M_2a_2^2)=\frac{M_1M_2}{M}a^2\Omega.}
$$

Using [Kepler's third law](../../../../../kepler-s-third-law.md), $\Omega^2=GM/a^3$, also gives $J=M_1M_2\sqrt{Ga/M}$. Under [conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md), $M$ and $J$ stay fixed, so $a\propto(M_1M_2)^{-2}$. Since $d\log M_2/d\log M_1=-q$, the [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) is

$$
\zeta_L=\frac{d\log R_L}{d\log M_1}=2(q-1)+\frac13=2q-\frac53.
$$

For the supplied giant response, luminosity stays fixed during the mass-loss perturbation and $\zeta_*=d\log R/d\log M_1=-0.27$. The change of the logarithmic overfill is $(\zeta_*-\zeta_L)d\log M_1$. Because the donor loses mass, this reduces overfill and stabilizes transfer precisely when $\zeta_*>\zeta_L$. Thus **the stated model requires**

$$
\boxed{q<q_{\rm crit}=\frac{5/3-0.27}{2}=0.6983\ldots\simeq0.7.}
$$

This is a response criterion within the given radius law; a different adiabatic donor response would change the dynamical threshold.

The initially more massive star evolves first. If it waits until it has the supplied giant structure while still having $q>1$, conservative overflow is unstable by this criterion. If [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) instead begins while the donor is on the [main sequence](../../../../../main-sequence.md) or shortly after central hydrogen exhaustion, its largely radiative-envelope response can allow transfer before a deep convective giant envelope develops. Mass loss and accretion can then reverse the mass ratio before it reaches the giant state. This is the [binary mass-ratio reversal](../../../../../binary-mass-ratio-reversal.md) route to an [Algol binary](../../../../../algol-binary.md), through [Case A mass transfer](../../../../../case-a-mass-transfer.md) or [early case B mass transfer](../../../../../early-case-b-mass-transfer.md).

At lobe filling, the lobe approximation and Kepler's law give the [pre-giant Roche-lobe-filling period limit](../../../../../pre-giant-roche-lobe-filling-period-limit.md)

$$
P=2\pi\sqrt{\frac{R_L^3}{0.462^3GM_1}}.
$$

It increases with the donor's radius. Requiring $R_L<R_{\rm BGB}=1.68R_\odot(M_1/M_\odot)^{5/3}$ therefore yields

$$
\boxed{P<P_0(M_1/M_\odot)^2,\qquad
P_0=2\pi\left(\frac{1.68}{0.462}\right)^{3/2}\sqrt{\frac{R_\odot^3}{GM_\odot}}\simeq0.8\ {
m d}.}
$$

The companion mass cancels in this lobe approximation.

Since $P\propto a^{3/2}$ at fixed total mass, the separation scaling gives **$\boxed{P(M_1M_2)^3=\text{constant}}$**. Use solar-unit masses $m_i=M_i/M_\odot$ and $m=m_1+m_2$, and let $K=P(m_1m_2)^3$. Then

$$
\frac P{m_1^2}=\frac K{m_1^5(m-m_1)^3},\qquad
\frac{d}{dm_1}\log(P/m_1^2)=-\frac5{m_1}+\frac3{m-m_1}.
$$

The derivative vanishes at $m_1=5m/8$, and its derivative is $5/m_1^2+3/(m-m_1)^2>0$, while the ratio diverges at both endpoints. Hence this is the global minimum, the [conservative pre-giant period-ratio minimum](../../../../../conservative-pre-giant-period-ratio-minimum.md).

For the stated Algol parameters, $m=4$ and $K=3(1\cdot3)^3=81$ days. At the minimum $m_1=2.5,m_2=1.5$, the period is $81/(2.5\cdot1.5)^3=1.536$ days and $P/m_1^2=0.24576$ days, well below $P_0=0.8$ days. This is a possible initially more-massive donor configuration with overflow before the giant branch. The current $q=1/3$ is also below the giant stability threshold. Thus **Algol is compatible with the proposed conservative early-overflow route**, although this necessary geometric test alone does not prove its full evolutionary history.

For RT Lac, $m=2.4$ and $K=5.1(0.9\cdot1.5)^3$. Its minimum occurs at $m_1=1.5,m_2=0.9$, where the mass product equals its current value, so $P=5.1$ days and

$$
\boxed{\min\frac P{m_1^2}=\frac{5.1}{1.5^2}=2.2667\ldots\ {
m d}>0.8\ {
m d}.}
$$

No conservative antecedent on this orbit can begin overflow before the giant branch. Beginning with an initially more massive giant instead encounters the instability just derived. **RT Lac cannot follow the stated coeval, conservative Algol-formation model.** A plausible alternative is rapid initial transfer with substantial mass and angular-momentum loss, via an outflow, strong wind or envelope-ejection episode. Such [nonconservative binary mass transfer](../../../../../nonconservative-binary-mass-transfer.md) changes both total mass and $J$ and removes the period-product constraint. Its present mass ratio $0.9/1.5=0.6$ permits stable current giant transfer. The given data do not determine a unique mass-loss history or establish a specific ejection mechanism.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
