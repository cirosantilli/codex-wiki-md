<h1 id="m/m4/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use independent colour marks, also independent of arrival times, as in the standard marked-process model. Let $K$ be the index of the first white arrival. Then $\mathbb P(K=k)=p(1-p)^{k-1}$ and $K$ is independent of the interarrival times. Thus $T=\sum_{j=1}^KX_j$. Conditional on $K$, [independence](../../../../../../independent-random-variables.md) makes its [moment-generating function](../../../../../../moment-generating-function.md) a power of $M_X$, and summing the [geometric series](../../../../../../geometric-series.md) gives

$$
M_T(\theta)=\sum_{k=1}^\infty p(1-p)^{k-1}\left(\frac\lambda{\lambda-\theta}\right)^k
=\boxed{\frac{p\lambda}{p\lambda-\theta}},\qquad\theta<p\lambda.
$$

This is the [exponential distribution](../../../../../../exponential-distribution.md) of rate $p\lambda$, so $T\sim\operatorname{Exp}(p\lambda)$. The calculation assumes $p>0$; if $p=0$, there is no white arrival and $T=+\infty$ almost surely.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [M4](../../../m4.md)
4. [M](../../../../m.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
