<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the [infinitesimal generator](../../../../../../infinitesimal-generator-stochastic-processes.md) be the second-order operator

$$
Lg(x)=\frac12\sum_{i,j=1}^d a_{ij}(x)\partial_{ij}g(x)+\sum_{i=1}^d b_i(x)\partial_i g(x),
$$

where $a(x)$ is symmetric positive semidefinite and $b(x)$ is a vector. In the standard bounded-coefficient setting take $a,b$ bounded and [measurable](../../../../../../measurability.md). An **[L-diffusion](../../../../../../diffusion-martingale-problem.md)** is a continuous [adapted process](../../../../../../adapted-process.md) $X$ for which, for every $g\in C_b^2(\mathbb R^d)$,

$$
\boxed{g(X_t)-g(X_0)-\int_0^t Lg(X_s)ds\text{ is a martingale}.}
$$

Here $C_b^2$ includes boundedness of the function and its derivatives through order two. This is the true-[martingale](../../../../../../martingale-split.md) version of the [diffusion martingale problem](../../../../../../diffusion-martingale-problem.md). The matrix $a$ is the diffusivity, and $b$ is the drift. An [Itô diffusion](../../../../../../ito-diffusion.md) with coefficient $\sigma$ has $a=\sigma\sigma^{\mathsf T}$.

A more general local [martingale problem](../../../../../../martingale-problem.md) may permit unbounded coefficients and require only a [local martingale](../../../../../../local-martingale.md). That convention is weaker and must not silently replace the true [martingale](../../../../../../martingale-split.md) property used here and in part (b). The bounded-coefficient convention guarantees all finite-horizon integrability needed below; a sufficient more general replacement is $\mathbb E\int_0^T(\sum_i|b_i(X_s)|+\sum_i a_{ii}(X_s))ds<\infty$ for every $T$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
