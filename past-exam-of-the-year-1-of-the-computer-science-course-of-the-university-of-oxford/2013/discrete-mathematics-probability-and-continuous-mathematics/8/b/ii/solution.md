<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume the [variances](../../../../../../variance-split.md) are finite. Expand the square and apply [linearity of expectation](../../../../../../linearity-of-expectation.md):

$$
\begin{aligned}
\operatorname{var}(X+Y)
&=\mathbb E[X^2]+2\mathbb E[XY]+\mathbb E[Y^2]-(\mathbb E[X]+\mathbb E[Y])^2\\
&=\operatorname{var}(X)+\operatorname{var}(Y)+2\bigl(\mathbb E[XY]-\mathbb E[X]\mathbb E[Y]\bigr).
\end{aligned}
$$

Part (i), applied to the identity [functions](../../../../../../function-split.md), makes the bracketed [covariance](../../../../../../covariance.md) zero by [independence of random variables](../../../../../../independent-random-variables.md). Hence

$$
\boxed{\operatorname{var}(X+Y)=\operatorname{var}(X)+\operatorname{var}(Y).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
