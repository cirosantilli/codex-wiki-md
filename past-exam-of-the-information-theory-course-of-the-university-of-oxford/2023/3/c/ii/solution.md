<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $0\leq q<1$, the number of attempts has the [geometric distribution](../../../../../geometric-distribution.md) with success [probability](../../../../../probability.md) $1-q$:

$$
\Pr(M_1=k)=q^{k-1}(1-q),\qquad k=1,2,\ldots.
$$

The [tail-sum formula for expectation](../../../../../tail-sum-formula-for-expectation.md) gives

$$
\boxed{\mathbb E M_1=\sum_{k=0}^{\infty}\Pr(M_1>k)=\sum_{k=0}^{\infty}q^k=\frac1{1-q}.}
$$

At $q=0$, $M_1=1$ deterministically. At $q=1$, $M_1=+\infty$ and its [expectation](../../../../../expected-value-split.md) is $+\infty$, rather than a finite waiting time.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
