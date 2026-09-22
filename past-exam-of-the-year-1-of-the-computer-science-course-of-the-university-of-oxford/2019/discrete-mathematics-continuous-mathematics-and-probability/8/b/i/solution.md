<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

This is a [Galton-Watson process](../../../../../../galton-watson-process-split.md) with offspring count $0$ with [probability](../../../../../../probability.md) $q=1-p$ and $2$ with [probability](../../../../../../probability.md) $p$. The descendants of distinct initial individuals evolve independently, so

$$
\alpha_i=\alpha_1^i
$$

for every finite initial size $i$. Conditioning on the first individual's outcome and applying the [law of total probability](../../../../../../law-of-total-probability.md) gives

$$
\alpha_1=q+p\alpha_2=q+p\alpha_1^2.
$$

The equation factors as

$$
(\alpha_1-1)(p\alpha_1-q)=0.
$$

Its roots are $1$ and $q/p$. Since $p<1/2$, the second root exceeds one and cannot be a [probability](../../../../../../probability.md). Therefore **$\alpha_1=1$ and $\alpha_i=1$ for every finite initial size**. The population reaches the absorbing state zero almost surely; no choice between two admissible fixed-point [probabilities](../../../../../../probability.md) remains in this subcritical case.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
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
