<h1 id="9/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since a square is nonnegative, $F_Y(y)=0$ for $y<0$. For $y\geq0$, the event $X^2\leq y$ is $-\sqrt y\leq X\leq\sqrt y$. As $X$ has no point masses,

$$
\boxed{F_Y(y)=\begin{cases}
0,&y<0,\\
F_X(\sqrt y)-F_X(-\sqrt y),&y\geq0.
\end{cases}}
$$

Differentiating for $y>0$ gives the contributions of the two inverse branches:

$$
\boxed{f_Y(y)=\begin{cases}
\dfrac{f_X(\sqrt y)+f_X(-\sqrt y)}{2\sqrt y},&y>0,\\
0,&y<0.
\end{cases}}
$$

The value assigned to the [probability density function](../../../../../../probability-density-function.md) at $y=0$ is arbitrary. It can be unbounded near $0$, but there is no atom there because $\mathbb P(X=0)=0$. Both positive and negative preimages must be included; keeping just one would generally lose probability.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
