<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each [random variable](../../../../../../random-variable-split.md), the [probability mass function](../../../../../../probability-mass-function.md) gives

$$
\mathbb E[X_i]=\frac{-1+0+1}{3}=0,
\qquad \mathbb E[X_i^2]=\frac{1+0+1}{3}=\frac23,
\qquad\operatorname{var}(X_i)=\frac23.
$$

Let $S_m=\sum_{i=1}^mX_i$. By [linearity of expectation](../../../../../../linearity-of-expectation.md) and [variance additivity for independent random variables](../../../../../../variance-additivity-for-independent-random-variables.md),

$$
\boxed{\mathbb E[S_m]=0,\qquad\operatorname{var}(S_m)=\frac{2m}{3}.}
$$

The [independence](../../../../../../independent-random-variables.md) is needed for the [variance](../../../../../../variance-split.md) calculation, but not for the [mean](../../../../../../expected-value-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
