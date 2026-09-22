<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [large-deviation speed](../../../../../../large-deviation-speed.md) $a_N=N^{1+\varepsilon}$ from part (a). For every $\eta>0$, the [Chernoff bound](../../../../../../chernoff-bound.md) for a [normal distribution](../../../../../../normal-distribution.md) gives, for all sufficiently large $N$,

$$
\mathbb P(|B_N|>\eta a_N)
\leq2\exp\!\left[-\frac{(\eta a_N-|N\mu|)^2}{2N\sigma^2}\right].
$$

Consequently

$$
\limsup_N a_N^{-1}\log\mathbb P(|B_N|>\eta a_N)=-\infty,
$$

because the exponent has order $N^{1+2\varepsilon}$, exceeding $a_N$ by a factor $N^\varepsilon$. Thus $(A+B_N)/a_N$ and $A/a_N$ satisfy [exponential equivalence](../../../../../../exponential-equivalence.md). This conclusion does not require [independence](../../../../../../independent-random-variables.md) between $A$ and $B_N$, since their difference is exactly $B_N/a_N$.

The [exponential equivalence](../../../../../../exponential-equivalence.md) theorem transfers the [large deviation principle](../../../../../../large-deviation-principle.md) and its [good rate function](../../../../../../good-rate-function.md), giving

$$
\boxed{\text{speed }N^{1+\varepsilon},\qquad I_{A+B}(x)=
\begin{cases}\lambda x,&x\geq0,\\+\infty,&x<0.\end{cases}}
$$

Large positive excursions are cheapest through the single [exponential random variable](../../../../../../exponential-distribution.md); a negative excursion would require the [Gaussian random variable](../../../../../../gaussian-random-variable.md) sum to move on its faster scale. If $\sigma=0$, the deterministic shift $N\mu/a_N\to0$ gives the same conclusion directly.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
