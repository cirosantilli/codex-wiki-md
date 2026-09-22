<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The sum still has a [normal distribution](../../../../../../normal-distribution.md), now with

$$
\mathbb E\frac{C+S_L}{L}=\mu+\frac{\nu}{L},\qquad
\operatorname{Var}\frac{C+S_L}{L}=\frac{\sigma^2}{L}+\frac{\rho^2}{L^2}.
$$

Its scaled [cumulant-generating function](../../../../../../cumulant-generating-function.md) is

$$
\frac1L\log\mathbb E e^{\theta(C+S_L)}
=\mu\theta+\frac{\sigma^2\theta^2}{2}+\frac{\nu\theta+\rho^2\theta^2/2}{L}.
$$

The limit is the same everywhere-finite function as in part (b), so the [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md) gives

$$
\boxed{I_C(x)=\frac{(x-\mu)^2}{2\sigma^2}}
$$

at [large-deviation speed](../../../../../../large-deviation-speed.md) $L$, when $\sigma^2>0$.

One can also see exactly why $C$ has no effect through [exponential equivalence](../../../../../../exponential-equivalence.md). For every $\varepsilon>0$, the [Chernoff bound](../../../../../../chernoff-bound.md) for the two [Gaussian tail bounds](../../../../../../gaussian-tail-bound.md) gives, when $L\varepsilon>|\nu|$ and $\rho^2>0$,

$$
\mathbb P(|C|>L\varepsilon)\leq2\exp\left(-\frac{(L\varepsilon-|\nu|)^2}{2\rho^2}\right).
$$

Its logarithm divided by $L$ tends to $-\infty$. If $\rho^2=0$, this probability is eventually zero. The transfer result for [exponential equivalence](../../../../../../exponential-equivalence.md) says that coupled families whose distance exceeds each fixed positive tolerance with superexponentially small probability share a [large deviation principle](../../../../../../large-deviation-principle.md) with the same [good rate function](../../../../../../good-rate-function.md). Apply it to $(C+S_L)/L$ and $S_L/L$. This also covers $\sigma^2=0$, with the point-mass [rate function](../../../../../../rate-function.md) from part (b).

## ↑ Ancestors (11)

1. [D](../d.md)
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
