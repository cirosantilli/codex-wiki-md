<h1 id="a/2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There are exactly $n$ summands in $S_n$, and the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\mathbb E\left|\frac{S_n}{n}-1\right|
\leq\frac1n\sum_{i=2}^{n+1}\mathbb E|X_i-1|
=\frac1n\sum_{i=2}^{n+1}\frac1{\log i}\longrightarrow0.
$$

The last step is convergence of arithmetic means of a sequence tending to zero. Thus $S_n/n\to1$ in $L^1$, and [Markov's inequality](../../../../../../markov-s-inequality.md) gives

$$
\boxed{S_n/n\longrightarrow1\text{ in probability}.}
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
