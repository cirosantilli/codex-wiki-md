<h1 id="probability/8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $0\le s\le1$, condition on $N=k$. Independence of the descendant [total progeny](../../../../../../../total-progeny-of-a-branching-process.md) variables gives

$$
\mathbb E\!\left[s^{\sum_{i=1}^N Z_i}\mid N=k\right]=\prod_{i=1}^k\mathbb E[s^{Z_i}]=G_Z(s)^k,
$$

including the empty product $1$ when $k=0$. Taking [expectation](../../../../../../../expected-value-split.md) over $N$ proves the [probability generating function of an independent random sum](../../../../../../../probability-generating-function-of-an-independent-random-sum.md) formula

$$
\boxed{\mathbb E\!\left[s^{\sum_{i=1}^N Z_i}\right]=\sum_{k=0}^\infty\mathbb P(N=k)G_Z(s)^k=G_N(G_Z(s)).}
$$

The same identity holds for complex $|s|<1$ by absolute convergence.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Probability](../../../../probability.md)
5. [Discrete mathematics, continuous mathematics, and probability](../../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../../split.md)
