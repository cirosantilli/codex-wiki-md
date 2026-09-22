<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the independent-site [Jukes-Cantor model](../../../../../jukes-cantor-model.md), the number of differences from a known ancestor has a [binomial distribution](../../../../../binomial-distribution.md) with mismatch probability

$$
p(t)=\frac34(1-e^{-\mu t}),\qquad d\sim\operatorname{Binomial}(L,p(t)).
$$

For an interior estimate, [maximum likelihood estimation](../../../../../maximum-likelihood-estimation-split.md) gives $\widehat p=d/L$. Equating this to the model probability and rearranging gives

$$
1-\frac{4d}{3L}=e^{-\widehat\mu t},\qquad\boxed{\widehat\mu=-\frac1t\ln\left(1-\frac{4d}{3L}\right)}.
$$

This is finite for $0\leq d/L<3/4$. At $d/L=3/4$, the estimate tends to infinity: the endpoint distribution has reached its limiting saturation and no finite rate can reproduce it exactly. For $d/L>3/4$, the displayed [logarithm](../../../../../logarithm.md) is not defined as a real number; within this model the constrained likelihood is maximized only as $\mu\to\infty$. For $d=0$ the boundary estimate is zero. The corresponding estimate of the actual event [mutation rate](../../../../../mutation-rate.md) is $\widehat r=3\widehat\mu/4$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
