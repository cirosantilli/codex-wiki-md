<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $S_L=X^{\oplus L}$. Its [Poisson distribution](../../../../../../poisson-distribution.md) has mean $L\lambda$, since the probability-generating functions of the independent summands multiply. Define

$$
Q_L=\frac{S_L-L\lambda}{L^{(1+\beta)/2}},\qquad a_L=L^\beta.
$$

The scaled [cumulant-generating function](../../../../../../cumulant-generating-function.md) is

$$
\Lambda_L(\theta)=\frac1{L^\beta}\log\mathbb E e^{L^\beta\theta Q_L}
=\lambda L^{1-\beta}\left(e^{\theta L^{(\beta-1)/2}}-1-\theta L^{(\beta-1)/2}\right).
$$

A [Taylor expansion](../../../../../../taylor-expansion.md) of the exponential, valid for each fixed $\theta$ because $\beta<1$, gives

$$
\Lambda_L(\theta)\longrightarrow\Lambda(\theta)=\frac\lambda2\theta^2.
$$

The remainder is $O(L^{(\beta-1)/2})$. The limit is finite and differentiable on all of $\mathbb R$, hence satisfies the essential-smoothness hypotheses of the [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md). Its [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) is

$$
\boxed{I_\beta(x)=\sup_\theta\{\theta x-\lambda\theta^2/2\}=\frac{x^2}{2\lambda}.}
$$

This proves the [Poisson moderate deviation principle](../../../../../../poisson-moderate-deviation-principle.md) with [large-deviation speed](../../../../../../large-deviation-speed.md) $L^\beta$ and a [good rate function](../../../../../../good-rate-function.md).

For an arbitrary [open set](../../../../../../open-set.md) $B$, the lower bound uses $\inf_BI_\beta$ and the upper bound uses $\inf_{\overline B}I_\beta$. These infima agree: every point of the closure is a limit of points of $B$ and $I_\beta$ is finite and continuous. Thus the [logarithmic probabilities of open sets for a continuous rate function](../../../../../../logarithmic-probabilities-of-open-sets-for-a-continuous-rate-function.md) give the stated logarithmic limit for every open $B$, not just intervals. The empty-set case follows from the usual infinite-value conventions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
