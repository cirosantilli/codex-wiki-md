<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [exponential series](../../../../../exponential-series.md) gives $x^x=e^{x\log x}=\sum_{k=0}^\infty(x\log x)^k/k!$. Since $|x\log x|\leq1/e$ on $(0,1)$, the [Weierstrass M-test](../../../../../weierstrass-m-test.md) proves [uniform absolute convergence](../../../../../uniform-absolute-convergence.md), using the summable bounds $e^{-k}/k!$. Therefore one can integrate the [series](../../../../../series-mathematics.md) term by term over this finite interval. Using part [i](../i.md),

$$
\int_0^1x^x\,dx=\sum_{k=0}^\infty\frac1{k!}\int_0^1(x\log x)^k\,dx
=\boxed{\sum_{k=0}^\infty\frac{(-1)^k}{(k+1)^{k+1}}.}
$$

This is the alternating identity in [sophomore's dream](../../../../../sophomore-s-dream.md). The same estimate also proves [absolute convergence](../../../../../absolute-convergence.md) of the integrated [series](../../../../../series-mathematics.md); no cancellation is needed to justify the interchange.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
