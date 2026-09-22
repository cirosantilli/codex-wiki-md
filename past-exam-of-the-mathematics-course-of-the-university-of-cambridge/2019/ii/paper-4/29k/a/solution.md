<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the one-period building block of the [Cox--Ross--Rubinstein model](../../../../../../cox-ross-rubinstein-model.md), the money-market account grows by a deterministic factor $R>0$, while the stock grows independently at each time by

$$
Y_t=\begin{cases}U,&\text{up},\\D,&\text{down},\end{cases}
\qquad 0<D<U.
$$

Thus $S_t^0=R^tS_0^0$ and $S_t^1=S_0^1\prod_{j=1}^tY_j$. Equivalently, the discounted stock has multipliers $u=U/R$ and $d=D/R$.

The model has no [arbitrage](../../../../../../arbitrage.md) precisely when the risk-free return lies strictly between the stock returns:

$$
\boxed{D<R<U,\qquad\text{equivalently}\qquad d<1<u.}
$$

Indeed, failure of either strict inequality gives a one-period arbitrage, while under the strict inequalities the probability

$$
\boxed{q=Q(Y_t=U)=\frac{R-D}{U-D}=\frac{1-d}{u-d}}
$$

lies in $(0,1)$. Taking the moves independent under $Q$ with up probability $q$ makes the discounted stock a [martingale](../../../../../../martingale-split.md), since $qu+(1-q)d=1$. This is the unique [Risk-neutral probability in the Cox--Ross--Rubinstein model](../../../../../../risk-neutral-probability-in-the-cox-ross-rubinstein-model.md), hence the unique equivalent martingale measure.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
