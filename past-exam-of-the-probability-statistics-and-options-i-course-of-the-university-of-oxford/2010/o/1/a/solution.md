<h1 id="o/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each before-and-after observation belongs to the same individual, so pairing removes individual baseline variation and allows dependence within a person's two readings. Under the stated independent normal model for the differences,

$$
\overline D\sim N(\mu,\sigma^2/n),\qquad
S_D^2=\frac1{n-1}\sum_{i=1}^n(D_i-\overline D)^2.
$$

The [independence of the normal sample mean and sample variance](../../../../../independence-of-the-normal-sample-mean-and-sample-variance.md) theorem gives [independence](../../../../../independent-random-variables.md) of $\overline D$ and $S_D^2$, and

$$
\boxed{c=\frac{n-1}{\sigma^2},\qquad cS_D^2\sim\chi^2_{n-1}.}
$$

Also $(\overline D-\mu)/(\sigma/\sqrt n)$ is standard normal. Dividing it by the square [root](../../../../../root-of-a-root-system.md) of the independent $\chi^2_{n-1}/(n-1)$ variable gives

$$
\boxed{Z=\frac{\overline D-\mu}{S_D/\sqrt n}\sim t_{n-1}.}
$$

Its law contains neither unknown parameter, providing the [pivotal quantity](../../../../../pivotal-quantity.md) for a [paired t-test](../../../../../paired-t-test.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
