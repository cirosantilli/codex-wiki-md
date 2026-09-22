<h1 id="9/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Differentiate the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) for $y>0$ using the [chain rule](../../../../../../chain-rule.md) and the [standard normal density](../../../../../../standard-normal-density.md):

$$
\begin{aligned}
f_Y(y)&=2\Phi'(\sqrt{2y})\frac1{\sqrt{2y}}\\
&=\frac{2}{\sqrt{2\pi}\sqrt{2y}}e^{-y}
=\frac{e^{-y}}{\sqrt{\pi y}}.
\end{aligned}
$$

Thus a [probability density function](../../../../../../probability-density-function.md) is

$$
\boxed{f_Y(y)=\begin{cases}
\dfrac{e^{-y}}{\sqrt{\pi y}},&y>0,\\
0,&y\le0.
\end{cases}}
$$

The value assigned at zero is immaterial. The [probability density function](../../../../../../probability-density-function.md) is unbounded near zero, but $F_Y(0)=0$ and continuity of the [cumulative distribution function](../../../../../../cumulative-distribution-function.md) there show that there is no point mass. This is a [gamma distribution](../../../../../../gamma-distribution.md) with shape $1/2$ and rate $1$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [9](../../../9.md)
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
