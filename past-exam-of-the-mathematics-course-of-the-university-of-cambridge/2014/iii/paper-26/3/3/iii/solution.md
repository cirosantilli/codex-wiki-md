<h1 id="3/3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $0<t<1$. The event $\{\tau\leq t\}$ means that the future path through time one never exceeds the maximum already attained by time $t$. Given $\mathcal F_t$, future increments form an independent [Brownian motion](../../../../../../../brownian-motion-split.md) $W$, so

$$
\mathbb P(\tau\leq t\mid\mathcal F_t)
=\mathbb P\left(\sup_{0\leq s\leq1-t}W_s\leq M_t-B_t\ \middle|\ \mathcal F_t\right)
=2\Phi\left(\frac{M_t-B_t}{\sqrt{1-t}}\right)-1.
$$

Here the [Brownian running maximum](../../../../../../../brownian-running-maximum.md) distribution is the one derived above. On $\{B_t<0\}$, an event of probability $1/2$, the finite quantity $M_t-B_t$ is strictly positive, so this [conditional probability](../../../../../../../conditional-probability.md) lies strictly between zero and one.

If $\tau$ were a [stopping time](../../../../../../../stopping-time.md), $\{\tau\leq t\}$ would be $\mathcal F_t$-measurable, and the displayed [conditional expectation](../../../../../../../conditional-expectation.md) of its indicator would equal that indicator, taking only zero and one. The contradiction proves **$\tau$ is not an $(\mathcal F_t)$-[stopping time](../../../../../../../stopping-time.md)**. Thus the [Strong Markov property](../../../../../../../strong-markov-property.md) cannot be invoked at $\tau$ to assert a Brownian shifted process; the direct argument here does not assume that property at this random time.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 26](../../../../paper-26-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
