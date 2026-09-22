<h1 id="a/2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Conditional on $\mathcal F_n$, the increment is $-X_n/2$ with probability $1-X_n$, and $(1-X_n)/2$ with probability $X_n$. Therefore

$$
\mathbb E((X_{n+1}-X_n)^2\mid\mathcal F_n)
=\frac{(1-X_n)X_n^2+X_n(1-X_n)^2}{4}
=\frac{X_n(1-X_n)}4.
$$

Taking expectations using the [tower property](../../../../../../law-of-total-expectation.md) yields

$$
\boxed{\mathbb E(X_{n+1}-X_n)^2=\tfrac14\mathbb E[X_n(1-X_n)].}
$$

This is the conditional variance that drives the [Bernoulli polarization martingale](../../../../../../bernoulli-polarization-martingale.md) toward its endpoints.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
