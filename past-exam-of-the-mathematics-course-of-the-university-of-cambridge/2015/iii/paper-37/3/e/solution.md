<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [autocovariance](../../../../../../autocovariance.md) vanishes beyond lag $q$. For an ordinary consecutive sum, [variance of a sum](../../../../../../variance-of-a-sum.md) gives

$$
\operatorname{Var}\!\left(\frac1{\sqrt n}\sum_{t=1}^nX_t\right)
=\sum_{|h|<n}\left(1-\frac{|h|}{n}\right)\gamma(h)
\longrightarrow\sum_{h\in\mathbb Z}\gamma(h).
$$

The last sum is finite. For $h\geq0$, $\gamma(h)=\sigma^2\sum_{j=0}^{q-h}\theta_j\theta_{j+h}$. Counting all coefficient pairs gives

$$
\boxed{\lim_{n\to\infty}\operatorname{Var}\!\left(\frac1{\sqrt n}\sum_{t=1}^nX_t\right)
=\sigma^2\left(\sum_{j=0}^q\theta_j\right)^2=\sigma^2\Theta(1)^2.}
$$

For the odd-indexed sample the lag-$h$ [autocovariance](../../../../../../autocovariance.md) is $\gamma(2h)$, so the same finite-sum argument gives $\sum_h\gamma(2h)$. Only coefficient pairs of the same parity contribute. If $E=\sum_{j\ {\rm even}}\theta_j$ and $O=\sum_{j\ {\rm odd}}\theta_j$, the **odd-subsample limit** is

$$
\boxed{\lim_{n\to\infty}\operatorname{Var}\!\left(\frac1{\sqrt n}\sum_{t=1}^nX_{2t-1}\right)
=\sigma^2(E^2+O^2)=\frac{\sigma^2}{2}\bigl[\Theta(1)^2+\Theta(-1)^2\bigr].}
$$

This is the [odd-subsample long-run variance of a moving average](../../../../../../odd-subsample-long-run-variance-of-a-moving-average.md). Equivalently it is $[f_X(0)+f_X(1/2)]/2$ in the cycles convention. Under the printed invertibility assumption and positive noise [variance](../../../../../../variance-split.md), the polynomial is nonzero at both $1$ and $-1$, so both limits are positive. The same formulas also hold without invertibility, when cancellations can make a limit zero.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
