<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\xi_t=\sqrt\kappa B_t$ and $0<\kappa<4$. We use these precise [Bessel process](../../../../../bessel-process.md) facts, which the question permits: for [dimension](../../../../../dimension-vector-space.md) $\delta>2$ a process started at $r>0$ exists for all time, never reaches zero, and has a strictly positive all-time minimum. More quantitatively,

$$
\mathbb P_r\left(\inf_{t\geq0}R_t\leq\varepsilon\right)
=(\varepsilon/r)^{\delta-2},\qquad0<\varepsilon<r.
$$

No assertion about [SLE](../../../../../schramm-loewner-evolution.md) simplicity or transience is being assumed.

For a real point $x>0$ before its Loewner lifetime, set $Z_t^x=g_t(x)-\xi_t$. Its equation is

$$
dZ_t^x=\frac2{Z_t^x}dt-\sqrt\kappa\,dB_t.
$$

Thus $Z^x/\sqrt\kappa$ is a [Bessel process](../../../../../bessel-process.md) of [dimension](../../../../../dimension-vector-space.md) $1+4/\kappa>2$. For each rational $x>0$ it stays positive on every finite interval, almost surely. These countably many events hold together. They cover every real $y>0$ as well: choose rational $0<x<y$ and observe that the noise cancels in the difference,

$$
g_t(y)-g_t(x)=(y-x)\exp\left(-2\int_0^t\frac{ds}{Z_s^yZ_s^x}\right)>0.
$$

Consequently $Z^y$ cannot reach zero while $Z^x$ remains positive. The negative side has the identical argument with the reflected [Brownian motion](../../../../../brownian-motion-split.md).

This excludes [Loewner trace](../../../../../trace-of-a-loewner-chain.md) contact with every real point other than zero, rather than just with each fixed rational point. On any finite interval a positive gap at a real point stays bounded away from zero. Continuous dependence of the [Chordal Loewner equation](../../../../../chordal-loewner-equation.md) then solves it on a complex neighborhood of that point, and the analytic flow extends the map conformally across a real interval there. Its real [derivative](../../../../../derivative.md) is $\exp(-2\int_0^t(Z_s^x)^{-2}ds)>0$, and its image stays away from the driving point. The [Loewner trace](../../../../../trace-of-a-loewner-chain.md) tip therefore cannot be there. We have proved $\gamma[0,\infty)\cap\mathbb R\subseteq\{0\}$.

Now use [Brownian motion](../../../../../brownian-motion-split.md) independent increments to restart at every deterministic rational time $s>0$. The centered future maps have [Loewner driver](../../../../../loewner-driving-function.md) $\xi_{s+t}-\xi_s$ and therefore the original [SLE](../../../../../schramm-loewner-evolution.md) law, independently of the past. Its [Loewner trace](../../../../../trace-of-a-loewner-chain.md) stays in $\mathbb H\cup\{0\}$ by the preceding argument. The inverse map $g_s^{-1}$ extends continuously to the real [boundary](../../../../../boundary-of-a-set.md) for a continuous trace-generated [compact H-hull](../../../../../compact-h-hull.md): the finite [Loewner trace](../../../../../trace-of-a-loewner-chain.md) gives a locally connected [boundary](../../../../../boundary-of-a-set.md), and the [Caratheodory boundary extension theorem](../../../../../caratheodory-boundary-extension-theorem.md) applies. Its value at $\xi_s$ is $\gamma(s)$. Thus the future in the original plane can meet $K_s\cup\mathbb R$ only at $\gamma(s)$. All these restart conclusions hold simultaneously for rational $s$.

Suppose $\gamma(u)=\gamma(v)$ with $u<v$. The [Loewner trace](../../../../../trace-of-a-loewner-chain.md) cannot be constant throughout $(u,v)$, since its [compact H-hull](../../../../../compact-h-hull.md) capacity increases strictly. By continuity there is a rational $s\in(u,v)$ with $\gamma(s)\ne\gamma(u)$. But $\gamma(v)=\gamma(u)$ lies in $K_s\cup\mathbb R$, contradicting the restart conclusion at $s$. This also excludes any return to the starting point. Hence **the [Loewner trace](../../../../../trace-of-a-loewner-chain.md) is simple and lies in the open [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) at every positive time**.

For transience, first strengthen the [boundary](../../../../../boundary-of-a-set.md) conclusion to avoidance of the [closure](../../../../../closure-topology.md) at each fixed real point. Fix $x>0$ and $0<r<x/4$. If the now-simple curve first enters the closed half-disc of radius $r$ about $x$ at time $\sigma$, join its tip to $x$ by the segment inside that disc. Before $\sigma$ the segment misses the [Loewner trace](../../../../../trace-of-a-loewner-chain.md). Together with the [Loewner trace](../../../../../trace-of-a-loewner-chain.md) and the real interval from zero to $x$, it bounds a pocket whose [boundary](../../../../../boundary-of-a-set.md) includes the positive side of the [Loewner trace](../../../../../trace-of-a-loewner-chain.md) and $[0,x/2]$. A [Brownian motion](../../../../../brownian-motion-split.md) path from high on the imaginary axis reaching that [boundary](../../../../../boundary-of-a-set.md) arc must enter the pocket through the segment. The [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md) bounds its [harmonic measure](../../../../../harmonic-measure.md) by the chance of hitting the entire half-disc.

The [boundary](../../../../../boundary-of-a-set.md) arc maps under $g_\sigma$ to $[\xi_\sigma,g_\sigma(x/2)]$. Its [harmonic measure](../../../../../harmonic-measure.md) from $iY$, as $Y\to\infty$, is

$$
\frac{g_\sigma(x/2)-\xi_\sigma}{\pi Y}+o(Y^{-1}).
$$

The half-disc maps out by $z\mapsto z+r^2/(z-x)$; its semicircle becomes an interval of length $4r$. Its [harmonic measure](../../../../../harmonic-measure.md) has asymptotic $4r/(\pi Y)$. Comparing and letting $Y\to\infty$ yields

$$
g_\sigma(x/2)-\xi_\sigma\leq4r.
$$

But $m_x=\inf_{t\geq0}(g_t(x/2)-\xi_t)>0$ by the [all-time minimum of a transient Bessel process](../../../../../all-time-minimum-of-a-transient-bessel-process.md) fact. The curve cannot enter any such disc with $4r<m_x$. Therefore it stays a strictly positive distance from $x$ for all time. Reflection proves the same for fixed $x<0$. This is the [boundary approach forces a small SLE Bessel gap](../../../../../boundary-approach-forces-a-small-sle-bessel-gap.md) argument; the [crosscut](../../../../../crosscut.md) comparison is also described in [the boundary-closure lemma in the primary SLE paper](https://arxiv.org/pdf/math/0106036).

Map out the simple initial slit at time one. The starting point zero has two distinct real [prime end](../../../../../prime-end.md) images $b_-,b_+$ under $g_1$, lying on opposite sides of $\xi_1$. Conditionally on the initial slit, the image future is a fresh independent [SLE](../../../../../schramm-loewner-evolution.md) translated by $\xi_1$. The just-proved fixed-point [closure](../../../../../closure-topology.md) avoidance applies to each of $b_--\xi_1$ and $b_+-\xi_1$. Therefore neither $b_-$ nor $b_+$ lies in the [closure](../../../../../closure-topology.md) of the mapped future. If a sequence of future [Loewner trace](../../../../../trace-of-a-loewner-chain.md) points approached zero in the original domain, their images would approach one of these two [prime ends](../../../../../prime-end.md). This is impossible. Thus

$$
R_1:=\inf_{t\geq1}|\gamma(t)|>0\quad\text{almost surely}.
$$

Finally [Scaling invariance of SLE](../../../../../scaling-invariance-of-sle.md) gives $R_T:=\inf_{t\geq T}|\gamma(t)|\overset d=\sqrt T R_1$. For every fixed $R>0$,

$$
\mathbb P(R_T\leq R)=\mathbb P(R_1\leq R/\sqrt T)\longrightarrow0.
$$

The events of returning to the closed radius-$R$ disc after time $T$ decrease as $T$ increases. Continuity of probability on decreasing events implies that the probability of returns at arbitrarily late times is zero. Taking the countable intersection over positive integer $R$ proves

$$
\boxed{\gamma\text{ is simple and }|\gamma(t)|\longrightarrow\infty\quad\text{almost surely}.}
$$

This proves actual eventual escape, not merely unboundedness of the growing [compact H-hulls](../../../../../compact-h-hull.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
