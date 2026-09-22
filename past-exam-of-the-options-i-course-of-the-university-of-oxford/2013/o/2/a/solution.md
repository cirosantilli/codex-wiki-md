<h1 id="o/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $s=\sum_{j=1}^nx_j$. The [Bernoulli distribution](../../../../../bernoulli-distribution.md) likelihood is proportional to $\theta^s(1-\theta)^{n-s}$. Multiplication by the [beta distribution](../../../../../beta-distribution.md) prior gives

$$
\pi(\theta\mid x)\propto\theta^{a+s-1}(1-\theta)^{b+n-s-1}.
$$

Normalizing with the [beta function](../../../../../beta-function.md) therefore gives

$$
\boxed{\theta\mid x\sim\operatorname{Beta}(a+s,b+n-s),\qquad\pi(\theta\mid x)=\frac{\theta^{a+s-1}(1-\theta)^{b+n-s-1}}{B(a+s,b+n-s)}.}
$$

The parameters remain positive. This is [Beta-binomial conjugacy](../../../../../beta-binomial-conjugacy.md): successes add to the first shape parameter and failures to the second.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [O](../../../o.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
