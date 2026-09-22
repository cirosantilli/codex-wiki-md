<h1 id="9/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since $X\geq0$, the [function](../../../../../../function-split.md) $X\mapsto X^2$ is [strictly increasing](../../../../../../strictly-increasing-function.md) on its support. For $y\geq0$,

$$
F_Y(y)=\mathbb P(X^2\leq y)=F_X(\sqrt y)=1-e^{-y/2},
$$

and $F_Y(y)=0$ for $y<0$. Differentiating the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) gives

$$
\boxed{f_Y(y)=\begin{cases}\tfrac12e^{-y/2},&y\geq0,\\0,&y<0.\end{cases}}
$$

The density value at the single point $y=0$ is immaterial. Hence $Y$ has an [exponential distribution](../../../../../../exponential-distribution.md) with rate $1/2$. Direct [integration by parts](../../../../../../integration-by-parts.md), or its standard [expected value](../../../../../../expected-value-split.md), yields

$$
\boxed{\mathbb E[X^2]=\mathbb E[Y]=\int_0^\infty\frac y2e^{-y/2}\,dy=2.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
