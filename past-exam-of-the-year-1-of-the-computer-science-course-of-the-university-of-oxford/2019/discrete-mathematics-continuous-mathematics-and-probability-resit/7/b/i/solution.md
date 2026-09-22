<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $E_0$ be the expected additional flips when there is no immediately preceding tail, and $E_1$ the expectation when the preceding flip is a tail. A one-step [first-step analysis](../../../../../../first-step-analysis.md) gives

$$
E_0=1+\tfrac12E_0+\tfrac12E_1,\qquad E_1=1+\tfrac12E_0.
$$

Solving gives $E_1=4$ and **$\mathbb E[F]=E_0=6$**. To justify finiteness before manipulating these expectations, split the flips into independent two-flip blocks. Each block has probability $1/4$ of being $TT$; hence $\mathbb P(F>2m)\leq(3/4)^m$. This [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md) makes the [expectation](../../../../../../expected-value-split.md) finite. The state $E_1$ is essential because successive possible pairs overlap: the waiting time is not itself a [geometric distribution](../../../../../../geometric-distribution.md) with parameter $1/4$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
