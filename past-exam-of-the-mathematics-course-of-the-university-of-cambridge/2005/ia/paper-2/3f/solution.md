<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Normalize the [probability density function](../../../../../probability-density-function.md) using $u=t^c$:

$$
1=A_c\int_0^\infty t^{c-1}e^{-t^c}\,dt=\frac{A_c}{c}\int_0^\infty e^{-u}\,du,
\qquad \boxed{A_c=c.}
$$

The corresponding [Weibull distribution](../../../../../weibull-distribution.md) has [survival function](../../../../../survival-function.md)

$$
S_c(v)=P(X_c\geq v)=\int_v^\infty ct^{c-1}e^{-t^c}\,dt=e^{-v^c},\qquad v\geq0.
$$

Since the distribution is continuous, the choices $>$ and $\geq$ have the same [probabilities](../../../../../probability.md). The [conditional probability](../../../../../conditional-probability.md) is consequently

$$
P(X_c\geq s+t\mid X_c\geq t)=\frac{S_c(s+t)}{S_c(t)}=e^{-[(s+t)^c-t^c]}.
$$

For $s,t>0$ and $c>1$, the supplied inequality, applied to $s/t$, gives $(s+t)^c>t^c+s^c$. Taking exponentials yields

$$
\boxed{P(X_c\geq s+t\mid X_c\geq t)<e^{-s^c}=P(X_c\geq s).}
$$

This expresses the increasing [hazard function](../../../../../hazard-function.md) $h_c(t)=ct^{c-1}$: surviving to a later age shortens the remaining lifetime in this [conditional distribution](../../../../../conditional-distribution.md). At $c=1$ equality holds, as expected from the [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md) of the [exponential distribution](../../../../../exponential-distribution.md).

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
