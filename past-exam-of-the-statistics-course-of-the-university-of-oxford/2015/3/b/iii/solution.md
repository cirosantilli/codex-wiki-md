<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The denominator $\Phi(z)$ is positive, so

$$
B<\frac1{10}
\quad\Longleftrightarrow\quad
1-\Phi(z)<\frac1{10}\Phi(z)
\quad\Longleftrightarrow\quad
\Phi(z)>\frac{10}{11}.
$$

Strict increase of the [standard normal distribution](../../../../../standard-normal-distribution.md) function turns this into $z>\Phi^{-1}(10/11)$. Since the coefficient multiplying $\overline x$ in $z$ is positive, the rejection rule is precisely $\overline x>c$, with

$$
\boxed{c=\frac{\sigma\sqrt{\sigma^2+n\tau^2}}{n\tau}
\Phi^{-1}\!\left(\frac{10}{11}\right)
=\frac\sigma{\sqrt n}\sqrt{1+\frac{\sigma^2}{n\tau^2}}
\Phi^{-1}\!\left(\frac{10}{11}\right).}
$$

The [quantile](../../../../../quantile-function.md) is approximately $1.33518$. Equivalently, the rule requires [posterior probability](../../../../../posterior-probability.md) of $H_0$ below $1/11$, because its [prior odds](../../../../../prior-odds.md) are one. The calculation is an instance of the [Bayes factor for the sign of a normal mean](../../../../../bayes-factor-for-the-sign-of-a-normal-mean.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
