<h1 id="a/2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [martingale](../../../../../../martingale-split.md) is bounded in $L^2$, so the increment-square series from part (a)(ii) is finite. The identity just obtained implies $\sum_n\mathbb E[X_n(1-X_n)]<\infty$, hence $\mathbb E[X_n(1-X_n)]\to0$. By [almost sure convergence](../../../../../../almost-sure-convergence.md) and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md),

$$
\mathbb E[X_\infty(1-X_\infty)]=0.
$$

The integrand is nonnegative because $X_\infty\in[0,1]$. It must vanish almost surely, giving $X_\infty\in\{0,1\}$.

The [martingale](../../../../../../martingale-split.md) has constant expectation $a$. Its $L^2$ convergence implies $L^1$ convergence by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), and hence $\mathbb E X_\infty=a$. Therefore

$$
\boxed{\mathbb P(X_\infty=1)=a,\qquad\mathbb P(X_\infty=0)=1-a.}
$$

The limiting law is the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) with parameter $a$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
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
