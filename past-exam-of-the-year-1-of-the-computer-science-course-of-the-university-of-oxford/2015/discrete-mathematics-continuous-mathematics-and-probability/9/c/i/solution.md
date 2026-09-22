<h1 id="9/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [random variable](../../../../../../random-variable-split.md) $Y=Z^2/2$ is nonnegative, so its [cumulative distribution function](../../../../../../cumulative-distribution-function.md) is zero for $y<0$. If $y\ge0$, then

$$
\begin{aligned}
F_Y(y)&=\mathbb P(Z^2/2\le y)
=\mathbb P(-\sqrt{2y}\le Z\le\sqrt{2y})\\
&=\Phi(\sqrt{2y})-\Phi(-\sqrt{2y})
=2\Phi(\sqrt{2y})-1.
\end{aligned}
$$

The last step uses the [symmetry](../../../../../../symmetry-physics.md) of the [standard normal distribution](../../../../../../standard-normal-distribution.md), $\Phi(-z)=1-\Phi(z)$. Hence

$$
\boxed{F_Y(y)=\begin{cases}
2\Phi(\sqrt{2y})-1,&y\ge0,\\
0,&y<0.
\end{cases}}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
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
