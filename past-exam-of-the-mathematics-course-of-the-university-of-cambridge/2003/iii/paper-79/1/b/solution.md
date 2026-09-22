<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $S_L=\sum_{i=1}^LA_i$ and $Z_L=S_L/L$. The [cumulant-generating function](../../../../../../cumulant-generating-function.md) of one [normal random variable](../../../../../../gaussian-random-variable.md) is

$$
\kappa(\theta)=\log\mathbb E e^{\theta A_1}=\mu\theta+\frac{\sigma^2\theta^2}{2},\qquad \theta\in\mathbb R.
$$

[Cramér's theorem](../../../../../../cramer-s-theorem.md) states that empirical means of [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) whose [moment-generating function](../../../../../../moment-generating-function.md) is finite on a neighborhood of zero satisfy a [large deviation principle](../../../../../../large-deviation-principle.md) at the sample-size [large-deviation speed](../../../../../../large-deviation-speed.md), with [good rate function](../../../../../../good-rate-function.md) equal to the [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) of their [cumulant-generating function](../../../../../../cumulant-generating-function.md). Here that gives

$$
I(x)=\sup_{\theta\in\mathbb R}\left\{\theta(x-\mu)-\frac{\sigma^2\theta^2}{2}\right\}.
$$

For $\sigma^2>0$, differentiation gives the maximizing parameter $\theta=(x-\mu)/\sigma^2$, and hence

$$
\boxed{I(x)=\frac{(x-\mu)^2}{2\sigma^2}.}
$$

This [rate function](../../../../../../rate-function.md) tends to infinity as $|x|\to\infty$, so its finite [sublevel sets](../../../../../../sublevel-set.md) are [compact](../../../../../../compact-space.md). Equivalently, the [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md) applies because the limiting scaled [cumulant-generating function](../../../../../../cumulant-generating-function.md) is finite and differentiable everywhere; it is [lower semicontinuous](../../../../../../lower-semicontinuity.md) and [essentially smooth](../../../../../../essential-smoothness-of-a-convex-function.md), with no finite domain boundary at which to check steepness. If $\sigma^2=0$ is permitted, $Z_L=\mu$ deterministically and the [rate function](../../../../../../rate-function.md) is zero at $\mu$ and infinity elsewhere.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
