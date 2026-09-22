<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the exponential payoff, substituting $U=e^{\theta X}V$ gives $U_X=\theta U$, $U_{XX}=\theta^2U$, and $U_{\sigma X}=\theta e^{\theta X}V_\sigma$. Dividing the backward [partial differential equation](../../../../../../partial-differential-equation-split.md) by the nonzero factor $e^{\theta X}$ therefore gives the [exponential payoff transform PDE](../../../../../../exponential-payoff-transform-pde.md)

$$
\boxed{V_t+\left(A(\sigma)+\rho\theta\sigma B(\sigma)\right)V_\sigma
+\frac12B(\sigma)^2V_{\sigma\sigma}
+\frac12\theta(\theta-1)\sigma^2V=0.}
$$

The terminal value is

$$
\boxed{V(T,\sigma)=1.}
$$

The correlation changes the first-derivative coefficient, while the original drift of the log price combines with its variance to give $\theta(\theta-1)/2$ rather than $\theta^2/2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
