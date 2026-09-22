<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<p<1$, [independence](../../../../../independent-random-variables.md) of the remaining indicators gives

$$
\mathbb P(E_1\cap\{S_n=k\})=\binom{n-1}{k-1}p^k(1-p)^{n-k}
=\frac kn\mathbb P(S_n=k).
$$

Because $0<k<n$, the latter probability is positive for interior $p$. The two events are [independent events](../../../../../independent-events.md) exactly when their joint probability equals $p\mathbb P(S_n=k)$, which is equivalent to $p=k/n$.

At $p=0$ or $p=1$, the event $\{S_n=k\}$ is null, and a null event is independent of every event. Therefore the full answer, including the degenerate endpoints, is

$$
\boxed{p\in\left\{0,\frac kn,1\right\}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
