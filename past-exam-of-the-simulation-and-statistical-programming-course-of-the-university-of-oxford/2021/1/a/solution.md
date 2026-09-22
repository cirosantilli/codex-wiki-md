<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $s=\sigma^2\geq1$. The two [multivariate normal distribution](../../../../multivariate-normal-distribution.md) [probability density functions](../../../../probability-density-function.md) have ratio

$$
w(x)=\frac{p(x)}{q(x)}=s^{d/2}\exp\!\left[-\frac12(1-s^{-1})\|x\|^2\right].
$$

Here $\|x\|$ is the [Euclidean norm](../../../../euclidean-norm.md). Consequently the smallest [rejection sampling](../../../../rejection-sampling.md) envelope constant, and its acceptance [probability](../../../../probability.md), are

$$
\boxed{M_*=\sup_xw(x)=s^{d/2}=\sigma^d,\qquad \mathbb P(\mathrm{accept})=s^{-d/2}.}
$$

The supremum is attained at $x=0$; hence no smaller constant can dominate the ratio. Draw $Y\sim N(0,sI_d)$ and an [independent](../../../../independent-random-variables.md) $U$ from the [uniform distribution](../../../../continuous-uniform-distribution.md) on $(0,1)$. Accept $Y$ when

$$
\boxed{U\leq\exp\!\left[-\frac12(1-s^{-1})\|Y\|^2\right];}
$$

otherwise repeat with fresh [independent random variables](../../../../independent-random-variables.md). One can generate $Y=\sqrt s\,G$ using a [random vector](../../../../random-vector.md) $G$ with [independent](../../../../independent-random-variables.md) [standard normal distribution](../../../../standard-normal-distribution.md) coordinates.

For any [measurable set](../../../../measurable-set.md) $B$, the joint acceptance [probability](../../../../probability.md) is $\int_Bq(y)p(y)/(M_*q(y))\,dy=M_*^{-1}\int_Bp(y)\,dy$. Dividing by $1/M_*$ proves that the returned [random vector](../../../../random-vector.md) has [probability density function](../../../../probability-density-function.md) $p$. The number of proposals has a [geometric distribution](../../../../geometric-distribution.md) on the positive integers, with [expected value](../../../../expected-value-split.md) $M_*$. When $s=1$, every proposal is accepted.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../split.md)
5. [Simulation and statistical programming course of the University of Oxford](../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
