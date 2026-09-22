<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Translate the centre of the ball to zero. Choose an inner radius $\rho$ strictly smaller than the ball's radius. If the starting point already lies in the ball there is nothing to prove; otherwise write $d=|z|>\rho$ and choose $R>d$. Let $H_\rho,H_R$ be the first hits of the two circles.

The [Brownian exit time](../../../../../../brownian-exit-time.md) from the annulus $\rho<|z|<R$ is finite almost surely: it is no later than exit of the first coordinate from $(-R,R)$, which is finite by part (a). The function $\log|z|$ is [harmonic](../../../../../../harmonic-function.md) on this annulus. The [Itô formula](../../../../../../ito-s-lemma.md) and [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) apply to its bounded stopped values, yielding

$$
\log d
=\mathbb P_z(H_\rho<H_R)\log\rho
+\mathbb P_z(H_R<H_\rho)\log R.
$$

Solving gives the [planar Brownian annulus hitting probability](../../../../../../planar-brownian-annulus-hitting-probability.md)

$$
\boxed{\mathbb P_z(H_\rho<H_R)=\frac{\log R-\log d}{\log R-\log\rho}.}
$$

As $R\to\infty$ this tends to one, while the event in the formula is contained in $\{H_\rho<\infty\}$. Thus the inner circle is hit almost surely. That circle lies strictly inside the original open ball, proving the [recurrence of planar Brownian motion](../../../../../../recurrence-of-planar-brownian-motion.md) in the form requested:

$$
\boxed{\mathbb P_z(\text{hit the given nonempty open ball})=1.}
$$

A probability-one intersection over balls with rational centres and positive rational radii makes this conclusion simultaneous for all nonempty open balls, since every such ball contains one from that countable family.

**Using a smaller inner circle ensures an actual visit to the open ball, rather than only a hit of its boundary.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
