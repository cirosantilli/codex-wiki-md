<h1 id="o/o1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each before/after pair concerns the same individual, so subject-specific baseline blood [pressure](../../../../../pressure-split.md) can affect both measurements. Analyzing the within-person difference retains this pairing and removes a common baseline contribution. Under the stated independent normal-difference model,

$$
\overline D\sim N(\mu,\sigma^2/n),\qquad
S_D^2=\frac1{n-1}\sum_{i=1}^n(D_i-\overline D)^2.
$$

The normal-[sample variance](../../../../../sample-variance.md) identity gives

$$
\boxed{c=\frac{n-1}{\sigma^2},\qquad cS_D^2\sim\chi^2_{n-1}.}
$$

Moreover $\overline D$ and $S_D^2$ are independent, because the sample-mean projection and centered residual projection of a Gaussian vector are orthogonal and hence independent. Thus the standardized normal variable $N=\sqrt n(\overline D-\mu)/\sigma$ is independent of $U=(n-1)S_D^2/\sigma^2\sim\chi^2_{n-1}$. Consequently

$$
\boxed{\frac{\overline D-\mu}{S_D/\sqrt n}
=\frac N{\sqrt{U/(n-1)}}\sim t_{n-1}.}
$$

This distribution is free of both unknown parameters.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O1](../../o1.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
