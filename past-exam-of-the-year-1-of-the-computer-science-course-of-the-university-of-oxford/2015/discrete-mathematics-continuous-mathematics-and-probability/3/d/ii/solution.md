<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Count the final division producing zero as an iteration, and let the total be $n$. The terminal product $a_nb_n=0$ alone gives no useful bound. Instead apply (i) to each nonterminal product, which is a positive [integer](../../../../../../integer-split.md) and hence at least $1$.

If $n\ge2$, the penultimate product satisfies

$$
1\le a_{n-1}b_{n-1}<\frac{ab}{2^{n-1}},
\qquad n-1<\log_2(ab).
$$

As $n$ is an [integer](../../../../../../integer-split.md), this implies

$$
\boxed{n\le\lceil\log_2(ab)\rceil.}
$$

For $n=1$, the same bound holds since $a>b\ge1$ implies $ab\ge2$. In particular the [Euclidean algorithm](../../../../../../euclidean-algorithm.md) uses $O(\log a+\log b)$ divisions, in [big O notation](../../../../../../big-o-notation.md). The convention that includes the final zero-producing division explains the one-step offset in the argument.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
