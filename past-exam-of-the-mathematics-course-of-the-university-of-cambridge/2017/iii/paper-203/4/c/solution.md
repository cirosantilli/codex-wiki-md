<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [boundary](../../../../../../boundary-of-a-set.md) assertion is interpreted at positive finite times: a chordal [SLE](../../../../../../schramm-loewner-evolution.md) already starts on the [domain boundary](../../../../../../boundary-of-a-domain.md), and its marked target is another [boundary](../../../../../../boundary-of-a-set.md) point. The precise conclusion in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) is $\gamma(0,\infty)\subseteq\mathbb H$ almost surely.

For $0<\kappa\leq4$ and a fixed real $x>0$, the centered [Boundary-point Bessel flow for SLE](../../../../../../boundary-point-bessel-flow-for-sle.md) $V_t=g_t(x)-U_t$ solves

$$
dV_t=\frac2{V_t}\,dt-\sqrt\kappa\,dB_t.
$$

Thus $R_t=V_t/\sqrt\kappa$ is a [Bessel process](../../../../../../bessel-process.md) driven by $-B$ of dimension

$$
\boxed{\delta=1+\frac4\kappa\geq2.}
$$

The [Hitting-zero classification for a Bessel process](../../../../../../hitting-zero-classification-for-a-bessel-process.md) says that, started positively, it never hits zero when $\delta\geq2$. For $x<0$, reflect the equation and apply the same result. Therefore every fixed nonzero [boundary](../../../../../../boundary-of-a-set.md) point has infinite swallowing time. A countable intersection gives this simultaneously for all nonzero rational [boundary](../../../../../../boundary-of-a-set.md) points.

To extend this countable conclusion to every real $x>0$, choose rational $q$ with $0<q<x$. The difference of two centered boundary solutions satisfies

$$
\frac{d}{dt}(V_t(x)-V_t(q))=-\frac{2(V_t(x)-V_t(q))}{V_t(x)V_t(q)},
$$

so it remains positive while both flows exist. On any finite time interval, $V_t(q)$ is bounded away from zero, hence so is $V_t(x)$. Moreover $V_t(x)=x-U_t+\int_0^t2/V_s(x)\,ds$ remains bounded there, so the differential equation continues for the whole interval. Its uniform separation from the [Loewner driving function](../../../../../../loewner-driving-function.md) also allows each flow map to continue as a [holomorphic function](../../../../../../holomorphic-function.md) on a complex [neighborhood](../../../../../../neighbourhood-mathematics.md) of $x$. Thus $x$ is outside $K_t$ and cannot be visited by the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md). Reflection gives the negative real axis. This uses countably many [Bessel processes](../../../../../../bessel-process.md) followed by deterministic flow comparison, rather than an uncountable union of probability-zero events.

To exclude a return to the starting point, use the [boundary extension of the inverse map for a continuous Loewner trace](../../../../../../boundary-extension-of-the-inverse-map-for-a-continuous-loewner-trace.md): $g_s^{-1}$ is continuous on the closed [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) and maps $U_s$ to $\gamma(s)$. This follows from the continuous trace theorem and the [Caratheodory boundary extension theorem](../../../../../../caratheodory-boundary-extension-theorem.md); it does not assume simplicity. At each deterministic rational time $s$, the [Conformal Markov property of SLE](../../../../../../conformal-markov-property-of-sle.md) makes the mapped future a fresh [SLE](../../../../../../schramm-loewner-evolution.md), so its trace lies in $\mathbb H\cup\{0\}$ by the preceding argument. Mapping back with $g_s^{-1}$ therefore shows

$$
\gamma[s,\infty)\cap(K_s\cup\mathbb R)\subseteq\{\gamma(s)\}.
$$

If a point $q=\gamma(r)$ were revisited at $t>r$, choose rational $s\in(r,t)$ with $\gamma(s)\ne q$. Such an $s$ exists because [continuity](../../../../../../continuous-function.md) and strictly increasing [half-plane capacity](../../../../../../half-plane-capacity.md) forbid a constant trace on an interval. But $q\in K_s\cup\mathbb R$, contradicting the displayed inclusion. This excludes all self-contacts, including returns to zero, and proves the [simple curve](../../../../../../simple-curve.md) property needed when discussing later swallowing times.

For $\kappa=0$, the deterministic [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) is $\gamma(t)=2i\sqrt t$, so the conclusion follows directly. Hence the [boundary-intersection threshold for SLE](../../../../../../boundary-intersection-threshold-for-sle.md) gives

$$
\boxed{\gamma(t)\in\mathbb H\text{ for every }t>0\text{ almost surely, for }0\leq\kappa\leq4.}
$$

Mapping to another marked [simply connected domain](../../../../../../simply-connected-domain.md) carries positive-time points into its [interior](../../../../../../interior-topology.md). The literal statement including the starting point is false, since $\gamma(0)$ is prescribed to be on the [domain boundary](../../../../../../boundary-of-a-domain.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
