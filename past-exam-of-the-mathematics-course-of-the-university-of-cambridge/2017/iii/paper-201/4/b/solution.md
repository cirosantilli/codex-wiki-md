<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix an exponent in the range from (a), and work on the single probability-one [event](../../../../../../event.md) where $K_\alpha<\infty$ and all dyadic values are finite. We give the [dyadic increment chaining](../../../../../../dyadic-increment-chaining.md) argument. For dyadic $s<t$, put $\delta=t-s$ and choose $n\geq0$ with $2^{-n}\leq\delta<2^{1-n}$. Let $s_j=2^{-j}\lfloor2^js\rfloor$ and $t_j=2^{-j}\lfloor2^jt\rfloor$. The level-$n$ approximations are at most two grid steps apart, so their difference is bounded by $2A_n$. At each subsequent level an approximation either stays fixed or moves by one adjacent level increment. Because $s,t$ are dyadic, these approximations eventually equal $s,t$. Thus

$$
|\xi_t-\xi_s|\leq2\sum_{j\geq n}A_j
\leq2^{-n\alpha}K_\alpha\leq K_\alpha|t-s|^\alpha.
$$

The [dyadic rationals](../../../../../../dyadic-rational.md) are dense in $[0,1]$, so this uniform bound gives a unique continuous extension $X$ to the entire interval, with

$$
\boxed{X_t=\xi_t\quad(t\in D),\qquad
|X_t-X_s|\leq K_\alpha|t-s|^\alpha.}
$$

All these equalities hold on that one [event](../../../../../../event.md), not merely one [event](../../../../../../event.md) per dyadic time. Define $X$ to be the zero path on its null complement. Each $X_t$ is measurable as the limit of the [random variables](../../../../../../random-variable-split.md) at deterministic left dyadic approximations. Alternatively, their measurable [linear interpolations](../../../../../../linear-interpolation.md) converge uniformly to $X$, which also shows measurability as a random element of $C([0,1])$. This is the continuous extension version of a [continuous modification](../../../../../../continuous-modification.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
