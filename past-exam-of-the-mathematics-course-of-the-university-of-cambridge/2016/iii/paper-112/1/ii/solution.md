<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First take nonempty bounded [open sets](../../../../../../open-set.md) $A,B\subset\mathbb R^n$. Their [Minkowski sum](../../../../../../minkowski-addition.md) is open and hence a [Lebesgue measurable set](../../../../../../lebesgue-measurable-set.md). Apply the [Prékopa–Leindler inequality](../../../../../../prekopa-leindler-inequality.md) to their [indicator functions](../../../../../../indicator-function.md) and the [indicator function](../../../../../../indicator-function.md) of $(1-\theta)A+\theta B$. This gives the multiplicative form

$$
\lambda_n((1-\theta)A+\theta B)\geq\lambda_n(A)^{1-\theta}\lambda_n(B)^\theta.
$$

To obtain the usual additive [Brunn–Minkowski inequality](../../../../../../brunn-minkowski-theorem.md), put $a=\lambda_n(A)^{1/n}$, $b=\lambda_n(B)^{1/n}$, $A_0=A/a$ and $B_0=B/b$. Both normalized [open sets](../../../../../../open-set.md) have [Lebesgue measure](../../../../../../lebesgue-measure.md) one. For $\theta=b/(a+b)$,

$$
\frac{A+B}{a+b}=(1-\theta)A_0+\theta B_0.
$$

The multiplicative bound and the scaling rule for [Lebesgue measure](../../../../../../lebesgue-measure.md) imply

$$
\boxed{\lambda_n(A+B)^{1/n}\geq\lambda_n(A)^{1/n}+\lambda_n(B)^{1/n}.}
$$

Replacing $A,B$ by $A\cap B(0,R),B\cap B(0,R)$ and using continuity from below extends this form of the [Brunn–Minkowski inequality](../../../../../../brunn-minkowski-theorem.md) to all nonempty [open sets](../../../../../../open-set.md), including those of infinite [Lebesgue measure](../../../../../../lebesgue-measure.md). This open-set form is sufficient here and avoids any measurability qualification for sums of arbitrary measurable sets.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
