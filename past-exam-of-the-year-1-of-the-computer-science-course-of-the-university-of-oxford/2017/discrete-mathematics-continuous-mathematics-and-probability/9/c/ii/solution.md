<h1 id="9/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The normalized sum has mean one and variance $(5n-2)/n^2$. For every fixed $\epsilon>0$, the [Chebyshev inequality](../../../../../../chebyshev-s-inequality.md) gives

$$
0\leq\mathbb P\left(\frac{S_n}{n}>1+\epsilon\right)
\leq\mathbb P\left(\left|\frac{S_n}{n}-1\right|>\epsilon\right)
\leq\frac{5n-2}{n^2\epsilon^2}\longrightarrow0.
$$

This proves the requested limit, and in fact proves [convergence in probability](../../../../../../convergence-in-probability.md) of $S_n/n$ to one. It is a [finite covariance range weak law](../../../../../../finite-covariance-range-weak-law.md): adjacent dependence is harmless here because only linearly many covariance terms survive.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
