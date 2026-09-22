<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $B$ be a standard [planar Brownian motion](../../../../../planar-brownian-motion.md) started at $z$. Neighbourhood recurrence means that, with [probability](../../../../../probability.md) one, every nonempty open subset of $\mathbb R^2$ is visited at arbitrarily large times. Not hitting points means that for each fixed $w\ne z$, $\mathbb P_z(\exists t\geq0:B_t=w)=0$. If $w=z$, time zero must be excluded, and there is still no return at any positive time. This assertion concerns each prescribed point; it does not say that the path contains no points.

We prove both claims from the [planar Brownian annulus hitting probability](../../../../../planar-brownian-annulus-hitting-probability.md). Fix a center $w$ and radii $0<r<\rho=|z-w|<R$, and define the [stopping times](../../../../../stopping-time.md) $\tau_r=\inf\{t:|B_t-w|=r\}$ and $\tau_R=\inf\{t:|B_t-w|=R\}$. Their minimum $\sigma$ is finite [almost surely](../../../../../almost-sure-convergence.md): a coordinate of [Brownian motion](../../../../../brownian-motion-split.md) cannot stay forever in a bounded interval, by the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md), so exit from the outer disk is finite. On the annulus,

$$
\Delta\log|x-w|=0.
$$

The [Itô formula](../../../../../ito-s-lemma.md) therefore makes $\log|B_{t\wedge\sigma}-w|$ a [local martingale](../../../../../local-martingale.md). It is bounded between $\log r$ and $\log R$, hence is a genuine [martingale](../../../../../martingale-split.md). The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $t\wedge\sigma$, followed by the [bounded convergence theorem](../../../../../bounded-convergence-theorem.md), gives

$$
\log\rho=\mathbb P_z(\tau_r<\tau_R)\log r+\mathbb P_z(\tau_R<\tau_r)\log R.
$$

Thus

$$
\boxed{\mathbb P_z(\tau_r<\tau_R)=\frac{\log(R/\rho)}{\log(R/r)}.}
$$

The exit can only be at one of the two distinct boundaries by path continuity.

For a fixed $r$, let $R\to\infty$. These events increase to $\{\tau_r<\infty\}$: any path up to a finite hitting time is bounded and so avoids some sufficiently large outer circle. The ratio tends to one, proving that any closed disk of positive radius is hit [almost surely](../../../../../almost-sure-convergence.md) from any starting point outside it. An initial point inside it already counts as a hit.

To prove the stronger recurrence statement, take a closed disk contained in any prescribed nonempty open set. At each integer time $n$, the [Markov property](../../../../../markov-property.md) and the preceding disk-hitting result imply that some time $t\geq n$ visits this disk with [probability](../../../../../probability.md) one. Intersecting these events over all $n$ proves visits at arbitrarily large times. A [countable](../../../../../countable-set.md) basis of disks with rational centers and rational radii makes this simultaneous for all nonempty open sets. This is [recurrence of planar Brownian motion](../../../../../recurrence-of-planar-brownian-motion.md), or equivalently neighbourhood recurrence.

For point avoidance, keep $R>\rho$ fixed and let $r\downarrow0$. Hitting $w$ before $\tau_R$ requires hitting every inner circle first. The displayed ratio tends to zero, so this point-hitting event has [probability](../../../../../probability.md) zero. Any finite hit of $w$ would occur before exit from some outer circle with integer radius, again because the preceding path is bounded. A [countable union](../../../../../countable-union.md) now gives $\boxed{\mathbb P_z(T_w<\infty)=0\ (z\ne w)}$, the [polar point for planar Brownian motion](../../../../../polar-point-for-planar-brownian-motion.md) assertion.

Finally, even if the process starts at $w$, for each deterministic $s>0$ its [normal distribution](../../../../../normal-distribution.md) has a density, so $\mathbb P(B_s=w)=0$. The [Markov property](../../../../../markov-property.md) at $s$ and the result from other starting points exclude any visit to $w$ at or after $s$. Taking $s=1/n$ excludes all positive-time returns. Thus **planar Brownian motion repeatedly approaches every point, while almost surely never hitting any prescribed point at positive time**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
