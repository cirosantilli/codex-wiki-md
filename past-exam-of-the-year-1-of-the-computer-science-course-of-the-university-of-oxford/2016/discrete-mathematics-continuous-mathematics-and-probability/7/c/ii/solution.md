<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives $S_n/n\to p$ in probability. If $\alpha<p$, the event $S_n/n\leq\alpha$ implies $|S_n/n-p|\geq p-\alpha$, whose probability tends to zero. If $\alpha>p$, its complement $S_n/n>\alpha$ implies $|S_n/n-p|>\alpha-p$, whose probability also tends to zero. Thus

$$
\boxed{\lim_{n\to\infty}\mathbb P(S_n/n\leq\alpha)=\begin{cases}0&\alpha<p,\\1&\alpha>p.\end{cases}}
$$

For an explicit independent bound, [Chebyshev's inequality](../../../../../../chebyshev-s-inequality.md) bounds either unwanted probability by $p(1-p)/[n(\alpha-p)^2]$. The boundary $\alpha=p$ is outside the two requested cases and is not decided by the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) alone.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
