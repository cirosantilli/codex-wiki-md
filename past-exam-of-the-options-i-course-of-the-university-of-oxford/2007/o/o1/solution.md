<h1 id="o/o1/solution">Solution</h1>

↑ **Parent:** [O1](../o1.md)

A frequentist [confidence interval](../../../../confidence-interval.md) is a pair of data-dependent endpoints whose random interval covers the fixed parameter with probability at least $1-\alpha$ under every allowed parameter value. In repeated uses of the same sampling procedure, at least the advertised fraction of intervals cover the true value. It is not a posterior probability assigned to the parameter after observing the data.

For a sample of size $n$ from a Poisson law with mean $\mu$, the sum $S$ is Poisson with mean $n\mu$. At observed $s>0$, define the lower and upper limits by

$$
\mathbb P_{nL}(S\ge s)=\alpha/2,\qquad
\mathbb P_{nU}(S\le s)=\alpha/2.
$$

At $s=0$ set $L=0$ and use the same upper equation. This inverts the two exact one-sided tail tests. Discreteness means the resulting central interval is generally conservative: its coverage is at least the nominal value, not identically equal to it.

Here one observes a four-year total of 39, so the lower endpoint satisfies $\phi_L(38)=0.975$ and the upper satisfies $\phi_U(39)=0.025$. Selecting the corresponding entries supplied in the source gives

$$
\boxed{[27.7,\ 53.3]}.
$$

This interval concerns the expected four-year total, not an annual rate. The other two supplied numbers correspond to the wrong inclusive tail for one of these endpoints.

## ↑ Ancestors (12)

1. [O1](../o1.md)
2. [O](../../o.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
