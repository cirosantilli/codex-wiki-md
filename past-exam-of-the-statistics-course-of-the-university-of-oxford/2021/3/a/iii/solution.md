<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [prior mean](../../../../../prior-mean.md) $1/(\beta+1)$ decreases as $\beta$ increases. More strongly, its [cumulative distribution function](../../../../../cumulative-distribution-function.md) and upper-tail [probability](../../../../../probability.md) are

$$
F_\beta(t)=1-(1-t)^\beta,\qquad
\mathbb P_\beta(\theta>t)=(1-t)^\beta,\qquad 0<t<1.
$$

For every fixed $t$, that upper-tail [probability](../../../../../probability.md) decreases with $\beta$. The statistician increasingly favors smaller values of $\theta$; as $\beta\to\infty$, the [prior distribution](../../../../../prior-probability.md) concentrates near zero. For $\beta>1$, its [variance](../../../../../variance-split.md) $\beta/[(\beta+1)^2(\beta+2)]$ also decreases. This is [concentration of a beta prior near zero](../../../../../concentration-of-a-beta-prior-near-zero.md).

With the data fixed, the [derivatives](../../../../../derivative.md) are

$$
\boxed{\frac{d\lambda}{d\beta}=\frac{N}{(N+\beta+1)^2}>0},\qquad
\boxed{\frac{d\widetilde\theta_1}{d\beta}
=-\frac{S+1}{(N+\beta+1)^2}<0}.
$$

Thus **the prior weight increases and the posterior mean decreases**. Their limits are $\lambda\to1$ and $\widetilde\theta_1\to0$. Both the changing [prior mean](../../../../../prior-mean.md) and the increasing weight contribute to the change in the [posterior mean](../../../../../posterior-mean.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
