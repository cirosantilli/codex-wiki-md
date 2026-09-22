<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Phase classification of the SLE trace](../../../../../../phase-classification-of-the-sle-trace.md) has its simple range

$$
\boxed{0\le\kappa\le4,}
$$

with $\kappa=0$ the deterministic vertical slit. For positive $\kappa$, the dividing parameter is precisely $\delta=1+4/\kappa=2$ in the [Boundary-point Bessel flow for SLE](../../../../../../boundary-point-bessel-flow-for-sle.md).

Here is the reason this diffusion threshold controls simplicity. For $\kappa\le4$, no nonzero real boundary point is swallowed. It suffices to check rational boundary points: a first meeting with either nonzero real half-axis would close a boundary crosscut and swallow a nonempty real interval, including a rational point. Thus the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) stays in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) apart from its starting point. By the [domain Markov property of a chordal Loewner chain](../../../../../../domain-markov-property-of-a-chordal-loewner-chain.md), after any fixed rational time $s$ the future mapped and centred [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) has the same boundary-avoidance property.

Suppose two [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) times $r<r'$ had the same image. Positive [half-plane capacity](../../../../../../half-plane-capacity.md) growth rules out constancy on a nonempty time interval, so continuity supplies a rational $s\in(r,r')$ with $\gamma_s\ne\gamma_r$. In the mapped future, the point at $r'$ is either in the open upper half-plane or at the starting boundary point $0$; it cannot lie at another real point. The first case puts $\gamma_{r'}$ inside the surviving domain at $s$, whereas $\gamma_r$ lies on the past [Loewner trace](../../../../../../trace-of-a-loewner-chain.md). The second gives $\gamma_{r'}=\gamma_s$, also contradicting the choice of $s$. Boundary continuity of the inverse [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) makes these identifications valid. This proves that the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) has no repeated points.

For $\kappa>4$, part (ii) makes a fixed positive real point have finite swallowing time, so the [SLE boundary swallowing criterion](../../../../../../sle-boundary-swallowing-criterion.md) ensures that the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) hits the positive real axis. In fact [positive boundary-interval hitting probability for SLE above parameter four](../../../../../../positive-boundary-interval-hitting-probability-for-sle-above-parameter-four.md) holds: any interval $J\subset(0,\infty)$ has positive hitting probability. To prove this, cover the positive axis by countably many dilates of $J$. If $J$ had zero hitting probability, [Scaling invariance of SLE](../../../../../../scaling-invariance-of-sle.md) would give zero probability for every dilate, contradicting the almost sure hit of the positive axis. Reflection gives the same conclusion for negative intervals.

At a fixed positive time, if the past [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) already repeats a point there is nothing to prove. Otherwise, boundary continuity of the inverse [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) supplies a nonempty real interval, away from the current driving point, mapped back into the earlier [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) in the open upper half-plane. Such an interval exists because positive capacity growth creates a genuine [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) boundary in the interior; choose an accessible boundary point away from the tip and then a small interval around its preimage. Conditional on the past, the [domain Markov property of a chordal Loewner chain](../../../../../../domain-markov-property-of-a-chordal-loewner-chain.md) gives a future centred SLE. With positive conditional probability its [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) hits this interval, by the preceding boundary-interval argument. Mapping back then gives a visit to the earlier [Loewner trace](../../../../../../trace-of-a-loewner-chain.md). Thus a repeated point occurs by some finite time with positive probability.

Finally let $E_t$ be the event of a repeated point by time $t$. [Scaling invariance of SLE](../../../../../../scaling-invariance-of-sle.md) makes $\mathbb P(E_t)$ the same for every $t>0$. The positive finite-time probability just proved makes this common value positive. Hence $\bigcap_nE_{1/n}$ also has positive probability. This event belongs to the Brownian germ sigma-field; the [Blumenthal zero-one law](../../../../../../blumenthal-zero-one-law.md) forces its probability to be one. Consequently **the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) is not simple almost surely for every $\kappa>4$**. At $\kappa=4$, the logarithmic scale function gives non-hitting of zero, so equality belongs to the simple range.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
