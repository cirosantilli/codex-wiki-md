<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $Y=Z^2/2$ is nonnegative, its [cumulative distribution function](../../../../../../../cumulative-distribution-function.md) is zero for $y<0$. For $y\geq0$,

$$
\begin{aligned}
F_Y(y)&=\mathbb P(Z^2\leq2y)=\mathbb P(-\sqrt{2y}\leq Z\leq\sqrt{2y})\\
&=\Phi(\sqrt{2y})-\Phi(-\sqrt{2y})=2\Phi(\sqrt{2y})-1.
\end{aligned}
$$

The last equality uses the symmetry of the [standard normal distribution](../../../../../../../standard-normal-distribution.md). Thus

$$
\boxed{F_Y(y)=\begin{cases}2\Phi(\sqrt{2y})-1,&y\geq0,\\0,&y<0.\end{cases}}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
