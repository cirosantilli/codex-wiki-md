<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $0\le t\le T$, set $Z_t=\cosh x\,Y_t$. Part (b) gives $Z_0=1$, $\mathbb EZ_T=1$, and $Z_t>0$. Its stochastic differential is

$$
dZ_t=Z_t\eta_t\,dW_t,\qquad\eta_t=-\tanh X_t.
$$

Thus $Z$ is the [stochastic exponential](../../../../../../doleans-dade-exponential.md) of $\int\eta\,dW$. The [Novikov condition](../../../../../../novikov-s-condition.md) also holds, since $\exp(\frac12\int_0^T\eta_t^2dt)\le e^{T/2}$.

The [Girsanov theorem](../../../../../../girsanov-theorem.md) says that under the measure with [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) $Z_T$, the process $W_t-\int_0^t\eta_sds$ is a [Brownian motion](../../../../../../brownian-motion-split.md) up to $T$. Substituting the sign of $\eta$ and the original [stochastic differential equation](../../../../../../stochastic-differential-equation.md) gives

$$
\boxed{W_t^{\mathbb Q}=W_t+\int_0^t\tanh X_s\,ds=X_t-x.}
$$

The density is strictly positive, so $\mathbb Q$ and $\mathbb P$ are [equivalent probability measures](../../../../../../equivalent-probability-measure.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
