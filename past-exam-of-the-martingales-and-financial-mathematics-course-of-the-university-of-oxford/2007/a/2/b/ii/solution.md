<h1 id="a/2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The summands are nonnegative, so [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), equivalently [Tonelli's theorem](../../../../../../tonelli-theorem.md) for a sum, gives

$$
\mathbb E\sum_{n=1}^\infty\left(\frac{S_n}{n}\right)^4
=\sum_{n=1}^\infty\frac{\mathbb ES_n^4}{n^4}
\leq3c^4\sum_{n=1}^\infty n^{-2}<\infty.
$$

A nonnegative [random variable](../../../../../../random-variable-split.md) with finite [expected value](../../../../../../expected-value-split.md) is finite almost surely. Thus the displayed nonnegative series converges almost surely, forcing its individual terms to tend to zero. Taking fourth roots proves

$$
\boxed{\frac1n\sum_{k=1}^nX_k\longrightarrow0
\quad\text{almost surely}.}
$$

This is a fourth-moment proof of a [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) for these bounded independent variables, without an identical-distribution assumption.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
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
