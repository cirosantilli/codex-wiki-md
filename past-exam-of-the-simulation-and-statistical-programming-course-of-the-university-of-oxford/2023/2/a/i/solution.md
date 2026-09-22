<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $w=p/q$ where $q>0$, assigning zero elsewhere. The envelope ensures $0\leq w/M\leq1$, and $\pi$ is nonnegative. Integrating its [joint probability density](../../../../../joint-probability-density.md) over the auxiliary coordinate gives

$$
\int_0^1\pi(x,u)\,du=Mq(x)\frac{w(x)}M=p(x).
$$

Consequently $\int_\Omega\int_0^1\pi(x,u)\,du\,dx=\int_\Omega p(x)\,dx=1$. This proves [normalization of a probability distribution](../../../../../normalization-of-a-probability-distribution.md); the change of integration order is justified by [Tonelli's theorem](../../../../../tonelli-theorem.md).

The coordinates are generally dependent. For $p(x)>0$, their [conditional probability density](../../../../../conditional-density.md) is

$$
\pi(u\mid x)=\frac M{w(x)}\mathbf1_{[0,w(x)/M]}(u).
$$

Thus $U\mid X=x$ has a [uniform distribution](../../../../../continuous-uniform-distribution.md) on an interval whose endpoint depends on $x$. They are [independent](../../../../../independent-random-variables.md) exactly when $w(x)$ is constant for $p$-almost every $x$, since only then do these conditional laws agree. In particular, $p=q$ is an exception: $X\sim p$ and $U\sim\operatorname{Unif}(0,1/M)$ are [independent](../../../../../independent-random-variables.md). An unconditional answer that they can never be [independent](../../../../../independent-random-variables.md) would therefore be too strong.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
