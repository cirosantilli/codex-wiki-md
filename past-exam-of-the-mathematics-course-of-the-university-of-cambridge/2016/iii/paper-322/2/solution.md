<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use a [circular orbit](../../../../../circular-orbit.md), as in the stated [Roche lobe](../../../../../roche-lobe.md) approximation, with orbital angular speed $\Omega$ and negligible stellar spin. The [center of mass](../../../../../center-of-mass.md) distances are $a_1=aM_2/M$ and $a_2=aM_1/M$. Summing the two orbital [angular momenta](../../../../../angular-momentum.md) gives

$$
\boxed{J=(M_1a_1^2+M_2a_2^2)\Omega=\frac{M_1M_2}{M}a^2\Omega.}
$$

[Kepler's third law](../../../../../kepler-s-third-law.md), $\Omega^2a^3=GM$, makes this $J=M_1M_2\sqrt{Ga/M}$. In [conservative mass transfer](../../../../../conservative-binary-mass-transfer.md), both $M$ and $J$ are fixed, while $dM_2=-dM_1$. Thus

$$
\frac{d\ln M_2}{d\ln M_1}=-q,\qquad \frac{d\ln a}{d\ln M_1}=2(q-1).
$$

The [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) is consequently

$$
\zeta_L=\frac{d\ln R_L}{d\ln M_1}=2(q-1)+\frac13=2q-\frac53.
$$

During a dynamical mass-loss perturbation, the deep interior and [luminosity](../../../../../luminosity.md) do not have time to change. The supplied giant structure therefore has [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md) $\zeta_*=-0.27$. Its fractional overfill changes by $d\ln(R/R_L)=(\zeta_*-\zeta_L)d\ln M_1$. The [binary mass ratio](../../../../../binary-mass-ratio.md) uses donor mass divided by accretor mass. Since $d\ln M_1<0$, self-limiting [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) requires $\zeta_*>\zeta_L$. Hence **the dynamical stability condition** is

$$
\boxed{q<q_{\mathrm{crit}}=\frac{5/3-0.27}{2}=0.698\overline3\simeq0.7.}
$$

At equality the linear restoring response vanishes. This [conservative mass-transfer critical mass ratio](../../../../../conservative-mass-transfer-critical-mass-ratio.md) uses the given radius exponent, rather than imposing the different fully convective $-1/3$ approximation.

The initially more massive component normally evolves first. If it first overflowed only after acquiring the given giant response, it would have $q>1$ and the mass loss would be dynamically unstable: its radius grows while its [Roche lobe](../../../../../roche-lobe.md) initially contracts. Starting overflow earlier can avoid this outcome. A [main sequence](../../../../../main-sequence.md) or early post-main-sequence [donor star](../../../../../donor-star.md) can have a radiative envelope with a stabilizing contraction response. Transfer then reverses the [binary mass ratio](../../../../../binary-mass-ratio.md) before the donor develops the giant structure. This is the route to an [Algol binary](../../../../../algol-binary.md) through [Case A mass transfer](../../../../../case-a-mass-transfer.md) during core hydrogen burning, or [early case B mass transfer](../../../../../early-case-b-mass-transfer.md) after core hydrogen exhaustion but before a deep giant envelope develops.

For the initial [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) to occur before the base of the giant branch, its lobe must be smaller than the base-of-branch stellar radius. Combining $R_L=0.462a(M_1/M)^{1/3}$ with [Kepler's third law](../../../../../kepler-s-third-law.md) cancels the companion dependence:

$$
P_i<2\pi\left[\frac{R_{\mathrm{BGB}}^3}{0.462^3GM_1}\right]^{1/2}.
$$

Writing $m_1=M_1/M_\odot$, substitute the [mass-radius relation](../../../../../mass-radius-relation.md) to obtain **the pre-giant period limit**:

$$
\boxed{P_i<P_0m_1^2,\qquad P_0=2\pi\left[\frac{(1.68/0.462)^3R_\odot^3}{GM_\odot}\right]^{1/2}\simeq0.803\,\mathrm{days}.}
$$

We use the specified $0.8\,\mathrm{days}$ below. This is a [pre-giant Roche-lobe-filling period limit](../../../../../pre-giant-roche-lobe-filling-period-limit.md), not a condition on the current stripped donor's radius.

At fixed total mass, [Kepler's third law](../../../../../kepler-s-third-law.md) gives $P\propto a^{3/2}$, while fixed orbital [angular momentum](../../../../../angular-momentum.md) gives $a\propto(M_1M_2)^{-2}$. Therefore **the conservative period invariant** is

$$
\boxed{P(M_1M_2)^3=\text{constant}.}
$$

To find the smallest possible pre-giant period ratio, use solar-unit masses $m_1,m_2$ and fixed $m=m_1+m_2$. Let $K=P(m_1m_2)^3$. Along this [period-product invariant for conservative mass transfer](../../../../../period-product-invariant-for-conservative-mass-transfer.md),

$$
F(m_1)=\frac{P}{m_1^2}=\frac K{m_1^5(m-m_1)^3}.
$$

The denominator has logarithmic derivative $5/m_1-3/(m-m_1)$, with a strictly negative derivative of its own. Its unique maximum, hence the unique minimum of $F$, occurs at

$$
\boxed{m_1=\frac58m,\qquad m_2=\frac38m.}
$$

Since $F$ diverges at either endpoint, this is the global [minimum period-to-donor-mass ratio for conservative evolution](../../../../../minimum-period-to-donor-mass-ratio-for-conservative-evolution.md).

For the quoted [Algol binary](../../../../../algol-binary.md), $K=3(1\times3)^3=81\,\mathrm{days}$ and $m=4$. Choosing the minimizing progenitor gives $m_{1,i}=2.5$, $m_{2,i}=1.5$ and

$$
P_i=\frac{81}{(2.5\times1.5)^3}=1.536\,\mathrm{days},\qquad F_{\min}=0.24576\,\mathrm{days}<0.8\,\mathrm{days}.
$$

Its pre-giant upper limit is $0.8(2.5)^2=5\,\mathrm{days}$, comfortably above this initial period. Subsequent [conservative mass transfer](../../../../../conservative-binary-mass-transfer.md) of $1.5M_\odot$ produces the stated masses and period. Thus **the data permit the proposed early-overflow formation route**.

For [RT Lac](../../../../../rt-lac.md), instead $K=5(0.5\times1.5)^3=2.109375\,\mathrm{days}$ and $m=2$. At its most favorable conservative progenitor, $m_{1,i}=1.25$, $m_{2,i}=0.75$ and

$$
P_i=2.56\,\mathrm{days},\qquad F_{\min}=1.6384\,\mathrm{days}>0.8\,\mathrm{days}.
$$

**No conservative progenitor meets the pre-giant overflow condition.** An initially more massive giant donor also fails the dynamical-stability condition derived above. Within this stable Algol-type formation model, the current RT Lac system therefore requires [nonconservative mass transfer](../../../../../nonconservative-binary-mass-transfer.md).

A plausible history is substantial envelope loss from the system, through a [stellar wind](../../../../../stellar-wind.md) or escaping overflow, possibly with a [common envelope](../../../../../common-envelope.md) episode. Escaping matter also carries orbital [angular momentum](../../../../../angular-momentum.md), so the total-mass and period-product invariants no longer constrain its initial orbit. A more massive progenitor can then shed its envelope and reach the present low donor mass without requiring the excluded conservative sequence. The supplied final data do not determine a unique mass-loss or angular-momentum-loss history.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
