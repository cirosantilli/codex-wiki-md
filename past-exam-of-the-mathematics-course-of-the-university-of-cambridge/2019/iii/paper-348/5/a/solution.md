<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $1\leq p<\infty$, define the [probability measures](../../../../../../probability-measure.md) with finite $p$th [absolute moment](../../../../../../absolute-moment.md) by

$$
\mathcal P_p(X)=\left\{\mu\in\mathcal P(X):\int_X|x-x_0|^p\,d\mu(x)<\infty\right\},
$$

where $x_0\in X$ is any fixed reference point. The condition is independent of the choice of $x_0$. The [p-Wasserstein distance](../../../../../../p-wasserstein-distance.md) is

$$
\boxed{d_{W_p}(\mu,\nu)=W_p(\mu,\nu)
=\left(\inf_{\pi\in\Pi(\mu,\nu)}\int_{X\times X}|x-y|^p\,d\pi(x,y)\right)^{1/p}.}
$$

The infimum is over all [transport plans](../../../../../../transport-plan.md), rather than only [transport maps](../../../../../../transport-map.md). The [product measure](../../../../../../product-measure.md) gives a finite upper bound using

$$
|x-y|^p\leq2^{p-1}\bigl(|x-x_0|^p+|y-x_0|^p\bigr).
$$

For $p=1$ this is the [Wasserstein distance](../../../../../../wasserstein-distance.md) with the metric of [Euclidean space](../../../../../../euclidean-norm.md); for $p=2$ it is the [second Wasserstein distance](../../../../../../second-wasserstein-distance.md). “Bounded moment” here means a finite integral, and does not require $X$ to be bounded.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
