<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $I$ be the number of heads in the initial allocation tosses. Then $I$ has the [binomial distribution](../../../../../../binomial-distribution.md) with parameters $n$ and $1/2$. Given $I=i$, the winning [probability](../../../../../../probability.md) is $i/n$, including the already finished games $i=0,n$. The [law of total probability](../../../../../../law-of-total-probability.md) and [linearity of expectation](../../../../../../linearity-of-expectation.md) give

$$
\begin{aligned}
\mathbb P(W)&=\sum_{i=0}^n\mathbb P(I=i)\frac in
=\frac{\mathbb E I}{n}
=\frac{n/2}{n}.
\end{aligned}
$$

Thus, for $n\ge1$,

$$
\boxed{\mathbb P(H\text{ finishes with all coins})=\frac12.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
