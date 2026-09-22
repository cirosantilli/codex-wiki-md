<h1 id="29j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $R=1+r$, $a=\mu-RS_0$, and $M=(\gamma V)^{-1}$. The terminal wealth is $W_1=Rw_0+\theta^T(S_1-RS_0)$, a [normal random variable](../../../../../../gaussian-random-variable.md) with mean $Rw_0+\theta^Ta$ and variance $\theta^TV\theta$. Its [moment-generating function](../../../../../../moment-generating-function.md) gives

$$
\mathbb E[-e^{-\gamma W_1}]=-\exp\left[-\gamma(Rw_0+\theta^Ta)+\frac{\gamma^2}{2}\theta^TV\theta\right].
$$

Maximizing this expected [exponential utility](../../../../../../constant-absolute-risk-aversion-utility.md) is equivalent to maximizing the strictly concave [quadratic form](../../../../../../quadratic-form.md) $\theta^Ta-(\gamma/2)\theta^TV\theta$. Since the nonsingular covariance $V$ is positive definite, the unique stationary point is the unique maximum:

$$
\boxed{\theta^*=M(\mu-RS_0),\qquad x^*=w_0-S_0^TM(\mu-RS_0).}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [29J](../../29j.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
