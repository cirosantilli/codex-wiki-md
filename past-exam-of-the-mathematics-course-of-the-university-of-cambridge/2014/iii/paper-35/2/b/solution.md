<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [binomial distribution](../../../../../../binomial-distribution.md), the [score function](../../../../../../informant-function.md) is

$$
\frac{Y}{\theta}-\frac{n-Y}{1-\theta}
=\frac{Y-n\theta}{\theta(1-\theta)}.
$$

Its squared [expected value](../../../../../../expected-value.md) is $I(\theta)=n/[\theta(1-\theta)]$, using the [binomial distribution](../../../../../../binomial-distribution.md) [variance](../../../../../../variance-split.md) $n\theta(1-\theta)$. Hence the [Jeffreys prior](../../../../../../jeffreys-prior.md) is

$$
\boxed{\pi_J(\theta)=\frac1{\pi\sqrt{\theta(1-\theta)}},\quad 0<\theta<1,}
$$

the [Beta distribution](../../../../../../beta-distribution.md) $\operatorname{Beta}(1/2,1/2)$. The factor $\sqrt n$ is independent of $\theta$ and disappears on normalization.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
