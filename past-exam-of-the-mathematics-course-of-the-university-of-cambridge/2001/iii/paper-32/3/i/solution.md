<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $K(t)=\log\mathbb E e^{tY}$ be the one-observation [cumulant-generating function](../../../../../../cumulant-generating-function.md), finite on an open interval containing zero. At a value $y$, find the real tilt $\widehat t$ solving

$$
K'(\widehat t)=y.
$$

If the distribution is nondegenerate then $K''(t)>0$ in the interior, so the solution is unique whenever $y$ is in the range of $K'$. The leading [saddlepoint density approximation](../../../../../../saddlepoint-density-approximation.md) to the [sample mean](../../../../../../sample-mean.md) is

$$
\boxed{\widehat f_{\bar Y}(y)=
\sqrt{\frac{n}{2\pi K''(\widehat t)}}
\exp\!\bigl(n\{K(\widehat t)-\widehat t y\}\bigr).}
$$

To derive it, use [exponential tilting](../../../../../../exponential-tilting.md):

$$
f_t(x)=e^{tx-K(t)}f_Y(x).
$$

Under this tilted distribution the mean is $K'(t)$ and the [variance](../../../../../../variance-split.md) is $K''(t)$, by differentiating its cumulant function $K(t+u)-K(t)$. For $S_n=\sum_iY_i$, changing measure gives the exact density identity

$$
f_{S_n}(ny)=e^{n\{K(t)-ty\}}f_{S_n,t}(ny).
$$

At $t=\widehat t$, $ny$ is the tilted mean. A local [normal approximation](../../../../../../normal-approximation.md) there gives $f_{S_n,\widehat t}(ny)\simeq(2\pi nK''(\widehat t))^{-1/2}$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) for $S_n=n\bar Y$ contributes the factor $n$, yielding the boxed formula.

This approximation retains the exponential large-deviation factor, while the curvature is evaluated at the tilt appropriate to each $y$. At the population mean, $\widehat t=0$, so it reduces to the usual central [normal approximation](../../../../../../normal-approximation.md). Under suitable smooth nonlattice transform-inversion conditions, its relative error at fixed interior $y$ is $O(n^{-1})$; existence of a few moments alone does not establish this density accuracy. Boundary values and absent exponential moments need separate treatment. The leading density need not integrate exactly to one, so it can be divided by its integral when a normalized approximation is desired.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
