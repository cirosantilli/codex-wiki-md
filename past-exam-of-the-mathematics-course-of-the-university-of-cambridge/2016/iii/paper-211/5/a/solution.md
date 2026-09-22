<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Backward induction makes every $U_t$ [adapted](../../../../../../adapted-process.md) and [integrable](../../../../../../integrability.md): the [conditional expectation](../../../../../../conditional-expectation.md) of an [integrable random variable](../../../../../../integrable-random-variable.md) is [integrable](../../../../../../integrability.md), and $|\max(a,b)|\leq|a|+|b|$. The [Snell envelope](../../../../../../snell-envelope.md) recursion directly gives $U_t\geq\mathbb E[U_{t+1}\mid\mathcal F_t]$, so $U$ is a [supermartingale](../../../../../../supermartingale.md).

If $Z$ is a [submartingale](../../../../../../submartingale.md), iterating its defining inequality gives $\mathbb E[Z_T\mid\mathcal F_t]\geq Z_t$. Starting at $U_T=Z_T$ and applying the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) backwards shows

$$
U_t=\max\{Z_t,\mathbb E[Z_T\mid\mathcal F_t]\}
=\mathbb E[Z_T\mid\mathcal F_t].
$$

This last [conditional expectation](../../../../../../conditional-expectation.md) is a true [martingale](../../../../../../martingale-split.md). **The conclusions are**

$$
\boxed{U\text{ is a supermartingale};\qquad
Z\text{ submartingale}\ \Longrightarrow\ U_t=\mathbb E[Z_T\mid\mathcal F_t]\text{ is a martingale}.}
$$

In the second case waiting until $T$ attains the [optimal stopping](../../../../../../optimal-stopping.md) value. It is not generally true that $U_t=Z_t$: that further equality holds when $Z$ itself is a [martingale](../../../../../../martingale-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
