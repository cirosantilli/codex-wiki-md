<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Represent the raindrops by a [Poisson random measure](../../../../../poisson-random-measure.md) on the space of location, impact time and [volume](../../../../../volume.md). Physical [volume](../../../../../volume.md) is nonnegative, so take the intensity density to vanish for $v<0$, or equivalently work on $\mathbb R^2\times\mathbb R\times[0,\infty)$ and extend it by zero to $\mathbb R^4$. Assume the radius function is measurable and nonnegative for elapsed times at least zero. Its stated monotonicity means patches grow rather than dry away.

A drop contributes to wetting $\xi$ at time $\tau$ precisely if its impact time is no later than $\tau$ and its current patch contains $\xi$. Thus define the deterministic [measurable set](../../../../../measurable-set.md)

$$
A_{\xi,\tau}=\{(x,t,v):t\le\tau,\ v\ge0,\ |x-\xi|\le r(\tau-t,v)\}.
$$

The number of covering drops is $\Pi(A_{\xi,\tau})$. Its [intensity measure of a point process](../../../../../intensity-measure-of-a-point-process.md) is

$$
m_{\xi,\tau}=\int_{-\infty}^{\tau}\int_0^\infty\int_{|x-\xi|\le r(\tau-t,v)}\lambda(x,t,v)\,dx\,dv\,dt.
$$

Since the point is dry if and only if that count is zero, the Poisson count definition gives the [void probability for growing Poisson rain patches](../../../../../void-probability-for-growing-poisson-rain-patches.md)

$$
\boxed{\mathbb P(\xi\text{ is dry at time }\tau)=\exp(-m_{\xi,\tau}).}
$$

Here $e^{-\infty}=0$: when the intensity is infinite, exhaust the covering set by increasing finite-intensity sets; their decreasing zero-count events have [probabilities](../../../../../probability.md) tending to zero. This also covers storms with infinitely many drops that can reach the point. The formula is valid for spatially inhomogeneous intensity. Only if the intensity is spatially constant may the spatial integral be replaced by $\pi r(\tau-t,v)^2$ times that intensity. Whether the circular boundary is included makes no difference for a density with respect to [Lebesgue measure](../../../../../lebesgue-measure.md), since each such boundary has zero spatial area. This construction is a time-dependent [Poisson germ-grain model](../../../../../poisson-germ-grain-model.md).

For total rainfall, the required general result is the [Campbell first-moment formula](../../../../../campbell-first-moment-formula.md): if $\Pi$ is a [Poisson random measure](../../../../../poisson-random-measure.md) with intensity $\mu$ and $h$ is any nonnegative measurable function, then

$$
\mathbb E\left[\int h(z)\,\Pi(dz)\right]=\int h(z)\,\mu(dz),
$$

with infinite values permitted. For a signed $h$, it holds with finite absolute [expectation](../../../../../expected-value.md) whenever $\int|h|d\mu<\infty$. No square-integrability hypothesis is required for this first-moment identity. The result is stated rather than proved, as allowed here.

The total rainfall [volume](../../../../../volume.md) is $V_{\rm total}=\sum_{(X,T,V)\in\Pi}V=\int v\,\Pi(dx\,dt\,dv)$, counting every drop once, independently of overlaps between its patch and other patches. Apply the stated formula with $h(x,t,v)=v$ on the physical mark space. Extending by zero to negative [volume](../../../../../volume.md) gives

$$
\boxed{\mathbb E[V_{\rm total}]=\int_{\mathbb R^4}v\lambda(x,t,v)\,dx\,dt\,dv.}
$$

If the displayed nonnegative integral is finite, the total [volume](../../../../../volume.md) is integrable and finite almost surely. If it is infinite, its [expectation](../../../../../expected-value.md) is infinite; this alone does not imply that the random total is infinite almost surely. The radius affects wet-area coverage but does not change this total-volume [expectation](../../../../../expected-value.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
