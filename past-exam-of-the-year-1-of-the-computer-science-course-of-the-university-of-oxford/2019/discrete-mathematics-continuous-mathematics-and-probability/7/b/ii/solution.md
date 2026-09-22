<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Split the unit square into $v\le u$ and $v>u$. The maximum is $u$ on the first triangle and $v$ on the second, so

$$
\begin{aligned}
\mathbb E[U\max\{U,V\}]
&=\int_0^1\left[\int_0^u u^2\,dv+\int_u^1 uv\,dv\right]du\\
&=\int_0^1\left[u^3+\frac u2(1-u^2)\right]du\\
&=\frac18+\frac14=\boxed{\frac38}.
\end{aligned}
$$

The shared boundary has zero [probability](../../../../../../probability.md), so it is not counted twice in this [joint density](../../../../../../joint-probability-density.md) calculation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
