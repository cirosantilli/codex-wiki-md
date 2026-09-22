<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A constant posterior [variance](../../../../../../variance-split.md) must be a fixed point of the recursion in part (b). Multiplying $P=V(P+W)/(P+W+V)$ by its positive denominator gives

$$
\boxed{P^2+PW=WV.}
$$

Conversely, if a nonnegative $P$ solves this equation and the filter is initialized with $P_0=P$, the recursion preserves $P_t=P$ at every step. The fixed-point equation alone does not force an arbitrary initial [covariance](../../../../../../covariance.md) to be constant.

For $W,V>0$, the admissible root and its [steady-state local-level Kalman gain](../../../../../../steady-state-local-level-kalman-gain.md) are

$$
P=\frac{\sqrt{W^2+4WV}-W}2,
\qquad K=\frac{P+W}{P+W+V}=\frac PV\in(0,1).
$$

The state estimate then obeys [exponential smoothing](../../../../../../exponential-smoothing.md):

$$
\boxed{\widehat S_t=KX_t+(1-K)\widehat S_{t-1}.}
$$

Iteration makes the weights explicit:

$$
\widehat S_t=(1-K)^t\widehat S_0
+K\sum_{j=0}^{t-1}(1-K)^jX_{t-j}.
$$

Thus older observations receive geometrically decreasing weights. Consistently with part (a), the innovations [variance](../../../../../../variance-split.md) is $q=P+W+V$ and the differenced MA coefficient is $\vartheta=-(1-K)$. The degeneracies $W=0,P=0$ and $V=0,P=0$ give gain zero and gain one respectively when the denominator is positive.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
