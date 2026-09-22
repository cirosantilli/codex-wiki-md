<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [prior mean](../../../../../prior-mean.md), [posterior mean](../../../../../posterior-mean.md), and [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) are

$$
\widetilde\theta_0=\frac1{\beta+1},\qquad
\widetilde\theta_1=\frac{S+1}{N+\beta+1},\qquad
\widehat\theta=\frac SN.
$$

For $0<S<N$, the last follows by maximizing $S\log\theta+(N-S)\log(1-\theta)$. At $S=0$ or $S=N$, use the usual [binomial likelihood](../../../../../binomial-likelihood.md) convention that admits the endpoints $0$ and $1$ as [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md); if the parameter domain is strictly $(0,1)$, these are boundary suprema rather than attained maxima. The [posterior mean](../../../../../posterior-mean.md) remains interior in all cases.

Taking

$$
\boxed{\lambda=\frac{\beta+1}{N+\beta+1}}
$$

gives

$$
\lambda\widetilde\theta_0+(1-\lambda)\widehat\theta
=\frac1{N+\beta+1}+\frac S{N+\beta+1}
=\boxed{\widetilde\theta_1}.
$$

Since $N=nm>0$ and $\beta+1>0$, **$0<\lambda<1$**. Thus the [posterior mean](../../../../../posterior-mean.md) is a [convex combination](../../../../../convex-combination.md) of the [prior mean](../../../../../prior-mean.md) and observed [binomial proportion](../../../../../binomial-proportion.md), with larger prior weight when $\beta+1$ is large relative to $N$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
