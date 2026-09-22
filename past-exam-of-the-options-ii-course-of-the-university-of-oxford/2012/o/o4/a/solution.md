<h1 id="o/o4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [sample mean](../../../../../sample-mean.md) has [expectation](../../../../../expected-value-split.md) $\theta$ and [variance](../../../../../variance-split.md) $\theta^2/n$. For $g(z)=\log z$, $g'(\theta)=1/\theta$. The first-order delta-method expansion is

$$
\log\overline Z\approx\log\theta+\frac{\overline Z-\theta}{\theta}.
$$

Taking its mean and [variance](../../../../../variance-split.md) gives

$$
\boxed{\mathbb E[\log\overline Z]\approx\log\theta,\qquad\operatorname{Var}(\log\overline Z)\approx\frac1n.}
$$

These are large-sample approximations. Retaining the quadratic Taylor term would add the leading mean correction $-1/(2n)$, but it does not change the requested first-order expression.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
