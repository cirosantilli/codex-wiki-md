<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

There are two necessary qualifications to the printed formula. **Critical points satisfy $g'=0$, not $g'=1$.** At a point with $g'=1$, the local degree is one and the printed summand is zero. In addition, $\log\|g'(0)\|$ is finite only when $g'(0)\ne0$; constant maps and origin-critical maps need separate treatment.

These are genuine issues even for otherwise ordinary disc maps. The map $g(z)=(z-1/2)^2/4$ maps the [unit disc](../../../../../unit-disc.md) into itself and has $g'(0)\ne0$. Its [derivative](../../../../../derivative.md) never equals one in the disc, so the printed count is zero, but it has a [ramification point](../../../../../ramification-point-of-a-holomorphic-map.md) at $1/2$ of [multiplicity](../../../../../multiplicity-mathematics.md) one. For $R>1/2$ the correct identity has the additional term $\log(2R)$, proving that the displayed identity with the literal printed count is false. Also $g(z)=z^2$ shows the undefined basepoint logarithm in an origin-critical example.

Prove the intended identity first for a nonconstant map with $g'(0)\ne0$. Let $H(z)=2|g'(z)|/(1-|g(z)|^2)$ be its [hyperbolic derivative density](../../../../../hyperbolic-derivative-density.md) and $u=\log H$. Away from [derivative](../../../../../derivative.md) zeros, $\log|g'|$ is harmonic, and direct differentiation gives

$$
\Delta[-\log(1-|g|^2)]=\frac{4|g'|^2}{(1-|g|^2)^2}=H^2.
$$

At a zero $a$ of $g'$ of [multiplicity](../../../../../multiplicity-mathematics.md) $m_a$, factor $g'=(z-a)^{m_a}h$ with $h(a)\ne0$. Its logarithm contains $m_a\log|z-a|$, whose distributional [Laplacian](../../../../../laplacian.md) is $2\pi m_a\delta_a$. Thus

$$
\Delta u=H^2+2\pi\sum_{g'(a)=0}m_a\delta_a.
$$

The local map degree is $m_a+1$, so this is the required excess-degree weighting.

For a smooth function, differentiating its circular mean and applying the [divergence theorem](../../../../../divergence-theorem.md) gives $\overline u'(r)=(2\pi r)^{-1}\int_{|z|<r}\Delta u\,dA$. Integrating in $r$ gives the logarithmic Green-Jensen formula. Factoring the isolated logarithmic singularities extends it to the present $u$:

$$
\frac1{2\pi}\int_0^{2\pi}u(Re^{i\theta})\,d\theta-u(0)
=\frac1{2\pi}\int_{|z|<R}\log\frac R{|z|}\,\Delta u\,dA.
$$

Substitution yields the [critical-point Jensen identity for the hyperbolic derivative](../../../../../critical-point-jensen-identity-for-the-hyperbolic-derivative.md)

$$
\boxed{T_{\mathbb D}(R)+N_{\rm crit}(R)=\frac1{2\pi}\int_0^{2\pi}\log H(Re^{i\theta})\,d\theta-\log H(0),}
$$

where $N_{\rm crit}=\sum_{|a|<R:g'(a)=0}m_a\log(R/|a|)$. This is the requested formula with the critical-point typo corrected. Initially choose a circle containing no [ramification point](../../../../../ramification-point-of-a-holomorphic-map.md) on its boundary; continuity and integrability of logarithmic boundary singularities extend the result to the remaining radii.

By [Schwarz-Pick theorem](../../../../../schwarz-pick-theorem.md), $H(z)\le2/(1-|z|^2)$. Therefore

$$
T_{\mathbb D}(R)+N_{\rm crit}(R)\le\log\frac2{1-R^2}-\log H(0).
$$

The normalized [hyperbolic distance](../../../../../hyperbolic-distance.md) is $\rho(R)=\log((1+R)/(1-R))$, and

$$
\log\frac2{1-R^2}=\rho(R)+\log2-2\log(1+R)\le\rho(R)+\log2.
$$

Consequently

$$
\boxed{T_{\mathbb D}(R)+N_{\rm crit}(R)\le\rho(R)+\log\frac2{H(0)}.}
$$

One can take $C_1=1$ and $C_2=\log(2/H(0))\ge0$. Since the corrected count is nonnegative in the noncritical-basepoint case, this also proves the growth bound for $T_{\mathbb D}$ with the literal printed, identically zero count, though not its false identity.

For completeness, if $g'$ vanishes to order $m\ge1$ at zero, put $c=\lim_{z\to0}H(z)/|z|^m>0$ and

$$
N_{\rm crit}^{\rm reg}(R)=m\log R+\sum_{0<|a|<R:g'(a)=0}m_a\log(R/|a|).
$$

Apply the same formula to $\log H-m\log|z|$, which is regular at zero. It gives

$$
\boxed{T_{\mathbb D}(R)+N_{\rm crit}^{\rm reg}(R)=\langle\log H\rangle_R-\log c\le\rho(R)+\log(2/c).}
$$

The origin contribution is a regularized Jensen term, not the undefined $\log(R/0)$. If one instead omits the origin term, the upper bound gains $-m\log R$; this is bounded for $R\ge1/2$, while the characteristic and off-origin count are bounded on any smaller compact disc. Thus a bound $C_1\rho+C_2$ still holds for that nonnegative-count convention after enlarging $C_2$. For a constant map $H=0$ and $T_{\mathbb D}=0$, so its characteristic growth bound is trivial; the logarithmic identity and a finite critical-divisor count are not defined. These qualifications resolve all maps allowed by the original opening sentence without asserting an undefined equality.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
