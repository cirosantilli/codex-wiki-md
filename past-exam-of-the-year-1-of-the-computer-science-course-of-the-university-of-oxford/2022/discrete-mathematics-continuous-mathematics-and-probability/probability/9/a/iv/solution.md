<h1 id="probability/9/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Because $Z=e^{-Y}>0$, its [cumulative distribution function](../../../../../../../cumulative-distribution-function.md) is zero for $z\le0$. For $z>0$, the transformation is decreasing, and $Y$ has a continuous [cumulative distribution function](../../../../../../../cumulative-distribution-function.md), so

$$
\mathbb P(Z\le z)=\mathbb P(Y\ge-\ln z)=1-F(-\ln z)=1-e^{-z}.
$$

Thus the [exponential transform of a standard Gumbel variable](../../../../../../../exponential-transform-of-a-standard-gumbel-variable.md) gives

$$
\boxed{F_Z(z)=\begin{cases}0,&z\le0,\\1-e^{-z},&z>0,\end{cases}\qquad Z\sim\operatorname{Exp}(1).}
$$

This is the [exponential distribution](../../../../../../../exponential-distribution.md) with rate $1$.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Probability](../../../../probability.md)
5. [Discrete mathematics, continuous mathematics, and probability](../../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../../split.md)
