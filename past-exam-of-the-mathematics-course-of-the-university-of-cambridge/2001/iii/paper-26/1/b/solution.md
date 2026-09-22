<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed $k$, [independence](../../../../../../independent-random-variables.md) and the [product large-deviation principle](../../../../../../product-large-deviation-principle.md) give the vector $(Y_n(1),\ldots,Y_n(k))$ the [good rate function](../../../../../../good-rate-function.md) $\sum_{j=1}^k I(y_j)$. Since the minimum is a [continuous map](../../../../../../continuous-map.md), the [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) gives

$$
J(m)=\inf_{\min_jy_j=m}\sum_{j=1}^kI(y_j).
$$

In every vector in this fibre, at least one coordinate equals $m$ and all others are at least $m$. The [large-deviation rate of a minimum of independent copies](../../../../../../large-deviation-rate-of-a-minimum-of-independent-copies.md) therefore reduces the infimum to

$$
J(m)=I(m)+(k-1)\inf_{y\ge m}I(y).
$$

If $0<m<\mu=\lambda^{-1}$, the other coordinates can equal $\mu$ and cost zero. If $m\ge\mu$, the [rate function](../../../../../../rate-function.md) is increasing on $[\mu,\infty)$, so every coordinate costs at least $I(m)$ and equality is achieved when all coordinates equal $m$. For $m\le0$ the cost is infinite. Thus

$$
\boxed{J(m)=\begin{cases}I(m),&m<\lambda^{-1},\\kI(m),&m\ge\lambda^{-1}.\end{cases}}
$$

At the threshold both expressions are zero. Goodness follows from the [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md). A small minimum requires only one atypically small mean; a large minimum requires all $k$ means to be atypically large, which explains the two costs.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
