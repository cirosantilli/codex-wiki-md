<h1 id="3g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First, compactness makes $X$ [totally bounded](../../../../../../totally-bounded-space.md): for every positive integer $k$, the open cover by balls of radius $1/k$ has a finite subcover. Given a sequence, repeatedly choose a ball of radius $1/k$ containing infinitely many terms of the subsequence retained at the preceding stage. Taking a diagonal subsequence $(x_{n_k})$, any two terms with indices at least $k$ lie in one ball of radius $1/k$, so their distance is below $2/k$. The diagonal subsequence is therefore a [Cauchy sequence](../../../../../../cauchy-sequence.md).

A compact metric space is [complete](../../../../../../complete-metric-space.md). To see this without assuming sequential compactness, let $(y_n)$ be Cauchy and put $F_n=\overline{\{y_m:m\geq n\}}$. These nonempty closed sets are nested and have the [finite intersection property](../../../../../../finite-intersection-property.md); compactness gives a point $y\in\bigcap_nF_n$. Given $\varepsilon>0$, a sufficiently late tail has diameter below $\varepsilon/2$, and because $y$ lies in its closure, every point of that tail lies within $\varepsilon$ of $y$. Thus $y_n\to y$.

The Cauchy subsequence constructed above consequently converges in $X$. Hence every compact metric space is sequentially compact.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3G](../../3g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
