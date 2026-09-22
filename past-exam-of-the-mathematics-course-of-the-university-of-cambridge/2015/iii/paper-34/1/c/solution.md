<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Conditioning on the intensity in the [Poisson mixture](../../../../../../poisson-mixture.md) gives

$$
G_N(z)=\mathbb E[e^{\Lambda(z-1)}]
=\left(\frac{p}{1-qz}\right)^2.
$$

Thus $N$ has the [negative binomial distribution](../../../../../../negative-binomial-distribution.md) with two successes and success probability $p$, counting failures; explicitly $\mathbb P(N=j)=(j+1)p^2q^j$ for $j\geq0$. The [probability generating function](../../../../../../probability-generating-function.md) is finite for real $z<1/q$.

The claim-size [moment-generating function](../../../../../../moment-generating-function.md) is $M_X(t)=(1-\mu t)^{-1}$. Substituting into the aggregate [moment-generating function](../../../../../../moment-generating-function.md) and using $p+q=1$ gives

$$
\boxed{M_S(t)=\left(\frac{p(1-\mu t)}{p-\mu t}\right)^2},
\qquad t<\frac p\mu.
$$

Put $L(t)=p/(p-\mu t)$, the [moment-generating function](../../../../../../moment-generating-function.md) of an [exponential distribution](../../../../../../exponential-distribution.md) with rate $p/\mu$. The identity

$$
\frac{p(1-\mu t)}{p-\mu t}=p+qL(t)
$$

then yields

$$
M_S(t)=p^2+2pqL(t)+q^2L(t)^2.
$$

The [gamma-mixed Poisson aggregate with exponential claims](../../../../../../gamma-mixed-poisson-aggregate-with-exponential-claims.md) has three nonnegative [mixture weights](../../../../../../mixture-weight.md) summing to one. By uniqueness of the [moment-generating function](../../../../../../moment-generating-function.md) near zero, **the aggregate distribution is**

$$
\boxed{\mathcal L(S)=p^2\delta_0+
2pq\,\operatorname{Exp}(p/\mu)+
q^2\,\operatorname{Gamma}(2,\text{rate }p/\mu).}
$$

Here $\delta_0$ is the [Dirac measure](../../../../../../dirac-measure.md) at zero. In particular $\mathbb P(S=0)=p^2$, consistently with $\mathbb P(N=0)$. The positive components have respective [expected values](../../../../../../expected-value.md) $\mu/p$ and $2\mu/p$; their [mixture distribution](../../../../../../mixture-distribution.md) accounts for the possibility of no aggregate payout.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
