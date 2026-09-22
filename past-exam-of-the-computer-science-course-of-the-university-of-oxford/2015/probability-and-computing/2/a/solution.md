<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each of the $b$ balls, let $I_i$ be the [indicator random variable](../../../../../indicator-random-variable.md) that ball $i$ survives the round of [uniform balls-in-bins allocation](../../../../../uniform-balls-in-bins-allocation.md). Condition on its chosen bin. Each of the other $b-1$ balls avoids that bin with [probability](../../../../../probability.md) $1-1/n$, independently, so the [probability](../../../../../probability.md) that ball $i$ is served is $(1-1/n)^{b-1}$. Hence, for $b\geq2$,

$$
\boxed{\mathbb E[\text{balls next round}\mid b]
=b\left[1-\left(1-\frac1n\right)^{b-1}\right].}
$$

We used [linearity of expectation](../../../../../linearity-of-expectation.md) to sum the [indicator random variables](../../../../../indicator-random-variable.md); their mutual [independence](../../../../../independent-random-variables.md) is unnecessary. For $b=0$ or $b=1$, the next count is zero. This states the boundary cases without an ambiguous $0^0$ when $n=1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
