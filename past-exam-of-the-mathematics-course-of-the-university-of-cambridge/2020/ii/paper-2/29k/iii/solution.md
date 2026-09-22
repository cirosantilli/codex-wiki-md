<h1 id="29k/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $Y_n=\log Z_n$ and

$$
\mu_*=\log(1+r)-\frac{\sigma^2}{2},
\qquad
\theta=\frac{\mu_*-\mu}{\sigma^2}.
$$

Define a probability measure $\mathbb P^*$ by the positive density

$$
\frac{d\mathbb P^*}{d\mathbb P}
=\prod_{k=1}^T
\exp\left\{
\theta(Y_k-\mu)-\frac12\theta^2\sigma^2
\right\}.
$$

The density has expectation one and is strictly positive, so $\mathbb P^*$ is equivalent to $\mathbb P$. By [exponential tilting](../../../../../../exponential-tilting.md), the variables $Y_k$ remain independent under $\mathbb P^*$ and have distribution $N(\mu_*,\sigma^2)$. Thus $Z_k$ has a [log-normal distribution](../../../../../../log-normal-distribution.md) and

$$
\mathbb E^*Z_k
=\exp\left(\mu_*+\frac{\sigma^2}{2}\right)
=1+r.
$$

For the discounted stock $\widetilde S_n=S_n/S_n^0$,

$$
\mathbb E^*(\widetilde S_n\mid\mathcal F_{n-1})
=\widetilde S_{n-1}\frac{\mathbb E^*Z_n}{1+r}
=\widetilde S_{n-1}.
$$

**Hence $\mathbb P^*$ is an [equivalent martingale measure](../../../../../../risk-neutral-measure.md).**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [29K](../../29k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
