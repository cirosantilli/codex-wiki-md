<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The two outcomes are not [independent](../../../../../../independent-random-variables.md).** Conditional on the selected die, the rolls are [independent](../../../../../../independent-random-variables.md), but sharing the unknown die creates [statistical dependence](../../../../../../statistical-dependence.md). Each nonfavored face has [probability](../../../../../../probability.md) $(1-1/2)/5=1/10$.

The unconditional [marginal distribution](../../../../../../marginal-distribution.md) assigns the following [probability](../../../../../../probability.md) to a $1$ on either roll:

$$
\mathbb P(X=1)=\mathbb P(Y=1)=
\frac16\left(\frac12+5\cdot\frac1{10}\right)=\frac16.
$$

However, by the [law of total probability](../../../../../../law-of-total-probability.md),

$$
\mathbb P(X=1,Y=1)=
\frac16\left[\left(\frac12\right)^2+
5\left(\frac1{10}\right)^2\right]=\frac1{20}\ne\frac1{36}.
$$

Thus the joint [probability](../../../../../../probability.md) does not factor into the two marginals. [Conditional independence](../../../../../../conditional-independence.md) given a shared latent choice does not imply unconditional [independence](../../../../../../independent-random-variables.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
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
