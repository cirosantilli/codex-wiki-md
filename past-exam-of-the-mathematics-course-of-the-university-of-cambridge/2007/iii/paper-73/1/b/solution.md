<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a constant-rate [Poisson process](../../../../../../poisson-process.md), let $T$ be the waiting time from a spike to the next spike. By [independent increments](../../../../../../independent-increments.md), there is no spike in an interval of length $u$ with probability $e^{-ru}$. Hence, for $r>0$,

$$
\boxed{F_T(u)=\mathbb P(T\leq u)=
\begin{cases}0,&u<0,\\1-e^{-ru},&u\geq0.\end{cases}}
$$

Its density is $re^{-ru}$, so the interspike intervals are independent [exponential distributions](../../../../../../exponential-distribution.md) with mean $1/r$. If $U$ is uniform on $(0,1)$, [inverse transform sampling](../../../../../../inverse-transform-sampling.md) gives $T=-\log U/r$. Repeatedly add independent draws to the current spike time to simulate a constant-rate [spike train](../../../../../../spike-train.md).

For a prescribed time-dependent nonnegative rate $r(t)$, use an [Inhomogeneous Poisson process](../../../../../../inhomogeneous-poisson-process.md). Conditional on the present event at $t_i$, its next waiting time has survival probability

$$
\mathbb P(T_i>u\mid t_i)=\exp\left[-\int_{t_i}^{t_i+u}r(s)\,ds\right].
$$

Thus its conditional CDF is $1$ minus that expression for $u\geq0$. Define the cumulative intensity $\Lambda(t)=\int_0^t r(s)\,ds$. For each new independent uniform draw, set $E_i=-\log U_i$ and solve

$$
\boxed{\Lambda(t_{i+1})-\Lambda(t_i)=E_i.}
$$

This transforms independent unit-rate exponential intervals in integrated-intensity time into physical spike times. Use a generalized inverse when the rate vanishes on an interval: no spikes are placed in a flat part of $\Lambda$. On a finite simulation window, stop when the next intensity target exceeds the available $\Lambda$. If the total future intensity is finite, a target beyond it means that no further spike occurs.

Numerically, integrate the known rate and invert the accumulated integral, or integrate exactly across piecewise-constant rate bins. **Drawing an exponential interval using only $r(t_i)$ is not exact when the rate changes during the interval.** The Poisson model also omits the [neuronal refractory period](../../../../../../neuronal-refractory-period.md) and other spike-history effects.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
