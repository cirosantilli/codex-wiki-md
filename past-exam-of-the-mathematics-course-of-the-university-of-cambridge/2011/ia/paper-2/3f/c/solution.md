<h1 id="3f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Construct independent copies $Y_1,Y_2,\ldots$ of $Y$, also independent of $X$, and define the [random sum](../../../../../../random-sum.md) $Z=\sum_{j=1}^X Y_j$, taking the empty sum to be zero. Independence gives, conditional on $X=n$,

$$
\mathbb E[e^{tZ}\mid X=n]=M_Y(t)^n.
$$

The [law of total expectation](../../../../../../law-of-total-expectation.md) gives the [transform composition for an independent random sum](../../../../../../transform-composition-for-an-independent-random-sum.md)

$$
\boxed{M_Z(t)=\sum_{n=0}^{\infty}\mathbb P(X=n)M_Y(t)^n=G_X(M_Y(t)).}
$$

The summands are nonnegative, so this equality is valid also as an extended-valued expectation. Where the right-hand side is finite, it is the ordinary [moment-generating function](../../../../../../moment-generating-function.md) of the constructed [random sum](../../../../../../random-sum.md). The construction does not assert a finite [moment-generating function](../../../../../../moment-generating-function.md) near zero for arbitrary $X,Y$: heavy tails can prevent this. For example a nonnegative $Y$ with no positive exponential moments and $X\equiv1$ already shows the necessary qualification.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3F](../../3f.md)
3. [Section I](../../section-i.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
