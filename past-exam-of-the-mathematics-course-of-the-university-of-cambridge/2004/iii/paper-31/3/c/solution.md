<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a common large threshold b, the header tail has exponent $-\log\rho$, whereas the payload tail has exponent $1-\rho$. Since $-\log\rho>1-\rho$ for $0<\rho<1$, **the payload [queue](../../../../../../queue-queueing-theory.md) has the heavier tail and dominates overflow on the large-buffer exponential scale at fixed load**. The inequality follows from the [strict convexity](../../../../../../strictly-convex-function.md) of minus the [logarithm](../../../../../../logarithm.md), or from integrating $1/u>1$ between rho and one.

The explanation is that a header always consumes one slot, while a payload can be unusually large. A rare accumulation of work can therefore overflow the byte buffer without accumulating as many as 1000 packets. Replacing every payload by its [mean](../../../../../../expected-value.md) would lose precisely this source of variability.

For the actual capacity 1000, retaining the exact continuous-time prefactors gives a qualification that a tail-exponent comparison alone cannot detect. The two infinite-buffer proxies are $p_H=\rho^{1000}$ and $p_P=\rho e^{-1000(1-\rho)}$, and

$$
\boxed{\log\frac{p_P}{p_H}=999(-\log\rho)-1000(1-\rho).}
$$

Thus payload overflow is more likely under this proxy exactly when the displayed expression is positive. For ordinary loads it is positive; for example it is positive at $\rho=0.9$. At $\rho=0.999$ it is approximately $-0.00050017$, so the header proxy is slightly larger. Consequently, without a numerical load, there is no universal exact ordering for the fixed capacity, although the large-buffer exponential ordering is unambiguous. Very near full utilization both 1000-unit buffers have substantial tail probabilities, so equal numerical capacities alone do not establish that the design is sensible. These are the requested infinite-space estimates, rather than an exact loss model for the interacting finite buffers.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
