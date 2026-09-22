<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [product large-deviation principle](../../../../../../product-large-deviation-principle.md) states that independent families satisfying [large deviation principles](../../../../../../large-deviation-principle.md) at the same speed with [good rate functions](../../../../../../good-rate-function.md) $J$ and $I$ have joint [good rate function](../../../../../../good-rate-function.md) $J(b)+I(z)$. The [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) states that a [continuous map](../../../../../../continuous-map.md) $f$ sends such a principle to one with [good rate function](../../../../../../good-rate-function.md) $\inf_{f(u)=x}I(u)$. Apply these results to $(B/L,S_L/L)$ and addition. The resulting [infimal convolution](../../../../../../infimal-convolution.md) is

$$
K(x)=\inf_{b\geq0}\left\{\lambda b+\frac{(x-b-\mu)^2}{2\sigma^2}\right\}.
$$

For $\sigma^2>0$, the unconstrained stationary point is $b=x-\mu-\lambda\sigma^2$. [Convexity](../../../../../../convex-function.md) gives the constrained minimum at $b_*=(x-\mu-\lambda\sigma^2)^+$, so

$$
\boxed{K(x)=\begin{cases}\dfrac{(x-\mu)^2}{2\sigma^2},&x\leq\mu+\lambda\sigma^2,\\\lambda(x-\mu)-\dfrac{\lambda^2\sigma^2}{2},&x\geq\mu+\lambda\sigma^2.\end{cases}}
$$

The two branches agree in value and first derivative at their junction. Both tails tend to infinity, giving a [good rate function](../../../../../../good-rate-function.md). This is the [fixed exponential perturbation of a Gaussian empirical mean](../../../../../../fixed-exponential-perturbation-of-a-gaussian-empirical-mean.md).

There is a reason to use the [product large-deviation principle](../../../../../../product-large-deviation-principle.md) rather than invoke the supplied [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md) without checking its hypotheses. The limiting scaled [cumulant-generating function](../../../../../../cumulant-generating-function.md) here is

$$
\Lambda(\theta)=\begin{cases}\mu\theta+\sigma^2\theta^2/2,&\theta<\lambda,\\+\infty,&\theta\geq\lambda.\end{cases}
$$

At $\lambda$ it is neither [lower semicontinuous](../../../../../../lower-semicontinuity.md) nor steep from the left: its left derivative tends to the finite value $\mu+\lambda\sigma^2$. Its [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) still equals $K$, but the stated [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md) does not establish the full lower bound on the linear branch. The [product large-deviation principle](../../../../../../product-large-deviation-principle.md) and [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) do establish it. In the degenerate case $\sigma^2=0$, the answer is $K(x)=\lambda(x-\mu)$ for $x\geq\mu$, and infinity otherwise.

## ↑ Ancestors (11)

1. [C](../c.md)
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
