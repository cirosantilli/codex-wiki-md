<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Subtracting the [expected value](../../../../../../expected-value.md) of $f$ does not alter either side, so suppose $\pi(f)=0$. Since reversibility makes $K$ a [self-adjoint operator](../../../../../../self-adjoint-operator.md) and stationarity makes it a contraction,

$$
\mathcal E_{K^2}(f)
=\lVert f\rVert_{L^2(\pi)}^2-\lVert Kf\rVert_{L^2(\pi)}^2.
$$

The [Discrete-time Poincaré inequality for a Markov kernel](../../../../../../discrete-time-poincare-inequality-for-a-markov-kernel.md) is therefore equivalent to

$$
\lVert Kf\rVert_2^2
\leq\left(1-\frac1C\right)\lVert f\rVert_2^2.
$$

Applying this inequality successively to $f,Kf,\ldots,K^{t-1}f$ yields

$$
\operatorname{Var}_\pi(K^tf)
=\lVert K^tf\rVert_2^2
\leq\left(1-\frac1C\right)^t
\lVert f\rVert_2^2
=\left(1-\frac1C\right)^t\operatorname{Var}_\pi(f).
$$

Conversely, the asserted variance contraction with $t=1$ rearranges to the Poincaré inequality. Hence the two statements are equivalent.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
