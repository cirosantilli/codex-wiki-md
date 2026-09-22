<h1 id="26k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Conditional expectation makes $Y_n$ measurable with respect to $\mathcal F_n$, and conditional Jensen gives $E|Y_n|\leq E|Y|<\infty$. The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) for nested sigma-algebras gives

$$
E[Y_{n+1}\mid\mathcal F_n]
=E[E[Y\mid\mathcal F_{n+1}]\mid\mathcal F_n]
=E[Y\mid\mathcal F_n]=Y_n.
$$

Thus this is a [martingale](../../../../../../martingale-split.md). **Its finite limit exists almost surely for every integrable $Y$ under the stated increasing [filtration](../../../../../../filtration-probability-theory.md)**: the [martingale](../../../../../../martingale-split.md) convergence theorem applies to the uniform bound on $E|Y_n|$. In fact the family is [uniformly integrable](../../../../../../uniform-integrability.md). One way to see this is to approximate $Y$ in $L^1$ by a bounded variable, whose [conditional expectations](../../../../../../conditional-expectation.md) remain bounded, while the [conditional expectations](../../../../../../conditional-expectation.md) of the error have uniformly small $L^1$ norm. Consequently convergence is also in $L^1$, with limit $E[Y\mid\sigma(\bigcup_n\mathcal F_n)]$. Mere [martingale](../../../../../../martingale-split.md) status without a suitable bound would not imply convergence.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [26K](../../26k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
