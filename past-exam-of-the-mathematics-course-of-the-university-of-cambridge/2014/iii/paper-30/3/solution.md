<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The ordinary column [Gram matrix](../../../../../gram-matrix.md) is $G=X^TX$. Use the normalized empirical [Gram matrix](../../../../../gram-matrix.md)

$$
\widehat\Sigma=\frac1nX^TX,
$$

so that standard Gaussian entries give $\mathbb E\widehat\Sigma=I_p$. This is the normalization needed for concentration around $\|\theta\|_2^2$.

The [restricted isometry property](../../../../../restricted-isometry-property.md) of order $s$ with constant $0\leq\delta<1$ means that the normalized map $X/\sqrt n$ approximately preserves the [Euclidean norm](../../../../../euclidean-norm.md) of all vectors with at most $s$ nonzero coordinates:

$$
(1-\delta)\|u\|_2^2\leq\frac1n\|Xu\|_2^2\leq(1+\delta)\|u\|_2^2.
$$

Equivalently, every principal block $\widehat\Sigma_{MM}$ with $|M|\leq s$ satisfies $\|\widehat\Sigma_{MM}-I\|_{\mathrm{op}}\leq\delta$. The least such $\delta$ is its [restricted isometry constant](../../../../../restricted-isometry-constant.md). In the unnormalized definition apply this property to $X/\sqrt n$ itself.

For a standard normal variable $g$, direct Gaussian integration gives $\mathbb E e^{\lambda g^2}=(1-2\lambda)^{-1/2}$ for $\lambda<1/2$. [Independence](../../../../../independent-random-variables.md) therefore yields the [moment-generating function of a chi-squared distribution](../../../../../moment-generating-function-of-a-chi-squared-distribution.md), centred here at its mean:

$$
\log\mathbb E e^{\lambda Z}=n\left(-\lambda-\tfrac12\log(1-2\lambda)\right)\leq\frac{n\lambda^2}{1-2\lambda},\qquad0\leq\lambda<\tfrac12.
$$

The inequality follows from $-\log(1-u)-u=\sum_{j\geq2}u^j/j\leq u^2/(2(1-u))$. For $t>0$, the [Chernoff bound](../../../../../chernoff-bound.md) with $\lambda=t/(2(n+t))$ gives

$$
\Pr(Z\geq t)\leq\exp\left(-\lambda t+\frac{n\lambda^2}{1-2\lambda}\right)=\exp\left(-\frac{t^2}{4(n+t)}\right).
$$

At $t=0$ the trivial [probability](../../../../../probability.md) bound suffices. This proves the requested bound, with a stronger prefactor one.

For the lower tail, $\log(1+u)\geq u-u^2/2$ gives $\log\mathbb E e^{-\lambda Z}\leq n\lambda^2$ for $\lambda\geq0$. Taking $\lambda=t/(2n)$ yields $\Pr(Z\leq-t)\leq e^{-t^2/(4n)}$. Combining both tails gives the useful [chi-squared concentration inequality](../../../../../chi-squared-concentration-inequality.md)

$$
\boxed{\Pr(|Z|\geq t)\leq2\exp\left(-\frac{t^2}{4(n+t)}\right),\qquad t\geq0.}
$$

For $z\geq0$ set $t=4(\sqrt{nz}+z)$. A direct calculation shows

$$
t^2-4z(n+t)=12nz+16z\sqrt{nz}\geq0.
$$

Thus the exponent is at least $z$, proving

$$
\boxed{\Pr(Z\geq4(\sqrt{nz}+z))\leq2e^{-z}.}
$$

The same threshold bounds the two-sided tail.

Finally fix a deterministic $\theta$ and put $r=\|\theta\|_2$. If $r>0$, [independence](../../../../../independent-random-variables.md) of the Gaussian rows gives $X_i\theta/r\sim N(0,1)$ independently. Therefore

$$
\theta^T\widehat\Sigma\theta=r^2\left(1+\frac Zn\right).
$$

The two-sided bound just proved supplies

$$
\boxed{\Pr\!\left(\left|\theta^T\widehat\Sigma\theta-\|\theta\|_2^2\right|>4\|\theta\|_2^2\left(\sqrt{\frac zn}+\frac zn\right)\right)\leq2e^{-z}.}
$$

For $r=0$ the [quadratic form](../../../../../quadratic-form.md) is deterministically zero; the strict inequality makes the formula valid in that case too. When $r\leq1$, replacing the threshold by $4(\sqrt{z/n}+z/n)$ gives an absolute bound [independent](../../../../../independent-random-variables.md) of $\theta$. In particular every fixed such direction concentrates at rate $n^{-1/2}$ for a fixed confidence level. The [restricted isometry property](../../../../../restricted-isometry-property.md) requires a simultaneous statement over sparse directions; this fixed-direction calculation alone is not that stronger assertion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
