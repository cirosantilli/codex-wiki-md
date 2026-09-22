<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If the initial individual has no offspring, $N=0$. If it splits, count that one event and the splitting events in its two [independent](../../../../../../independent-random-variables.md) descendant trees. Thus

$$
N=
\begin{cases}
0,&\text{with probability }q,\\
1+N_1+N_2,&\text{with probability }p,
\end{cases}
$$

where $N_1,N_2$ are [independent](../../../../../../independent-random-variables.md) copies of $N$. Taking the [probability generating function](../../../../../../probability-generating-function.md) gives

$$
G_N(s)=q+psG_N(s)^2.
$$

For $0<s\le1$, the quadratic equation has two algebraic branches. A [probability generating function](../../../../../../probability-generating-function.md) must remain finite at $s=0$, where it equals $\mathbb P(N=0)=q$, so the admissible branch is

$$
\boxed{G_N(s)=\frac{1-\sqrt{1-4pqs}}{2ps}
=\frac{2q}{1+\sqrt{1-4pqs}},\qquad G_N(0)=q.}
$$

The rationalized formula is also defined directly at zero. At $s=1$, $\sqrt{1-4pq}=q-p$, so $G_N(1)=1$, consistent with almost-sure finiteness. Extinction occurs after a finite number of generations almost surely, and each generation is finite, which justifies that finiteness claim for the [number of splitting events in a binary branching process](../../../../../../number-of-splitting-events-in-a-binary-branching-process.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
