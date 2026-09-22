<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Using the rate parameter convention for the [exponential distribution](../../../../../../exponential-distribution.md), [independence](../../../../../../independent-random-variables.md) gives the [joint probability density function](../../../../../../joint-probability-density.md)

$$
\boxed{f_{U,V}(u,v)=2e^{-u-2v}\mathbf1_{\{u\geq0,\ v\geq0\}}.}
$$

For $z\geq0$, the survival [probability](../../../../../../probability.md) of the minimum is

$$
\mathbb P(Z>z)=\mathbb P(U>z,V>z)=e^{-z}e^{-2z}=e^{-3z}.
$$

Thus **$Z$ has exponential distribution with rate $3$**, and

$$
f_Z(z)=3e^{-3z}\mathbf1_{\{z\geq0\}}.
$$

Values of a [probability density function](../../../../../../probability-density-function.md) at the single endpoint $0$ do not affect the [probability distribution](../../../../../../probability-distribution-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
