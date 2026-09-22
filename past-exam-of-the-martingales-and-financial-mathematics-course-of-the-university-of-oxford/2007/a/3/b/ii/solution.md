<h1 id="a/3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The products are nonnegative and measurable. [independence](../../../../../../independent-random-variables.md) and the unit means give $\mathbb EY_n=\prod_{k\leq n}\mathbb E\xi_k=1$, so they are integrable.

Let $\mathcal H_n=\sigma(Y_0,\ldots,Y_n)$ be the [natural filtration](../../../../../../natural-filtration.md). It is contained in $\sigma(\xi_1,\ldots,\xi_n)$, so $\xi_{n+1}$ is independent of $\mathcal H_n$ even if some products have vanished. Using the bounded or integrable nonnegative conditional-product identity,

$$
\mathbb E(Y_{n+1}\mid\mathcal H_n)
=Y_n\mathbb E(\xi_{n+1}\mid\mathcal H_n)
=Y_n.
$$

Thus **$Y$ is a [martingale](../../../../../../martingale-split.md) in its [natural filtration](../../../../../../natural-filtration.md)**.

Doob's convergence theorem in the form needed here states that a nonnegative [supermartingale](../../../../../../supermartingale.md) converges almost surely to a finite integrable limit; more generally a [submartingale](../../../../../../submartingale.md) with uniformly bounded first absolute moments has such an [almost sure convergence](../../../../../../almost-sure-convergence.md). Applying it to $Y$ gives

$$
\boxed{Y_n\to Y_\infty\text{ almost surely},\qquad
\mathbb E Y_\infty\leq1.}
$$

The [expected value](../../../../../../expected-value-split.md) bound follows from [Fatou's lemma](../../../../../../fatou-s-lemma.md). The theorem does not assert $L^1$ convergence or equality of [expected values](../../../../../../expected-value-split.md) without a uniform-integrability hypothesis.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
