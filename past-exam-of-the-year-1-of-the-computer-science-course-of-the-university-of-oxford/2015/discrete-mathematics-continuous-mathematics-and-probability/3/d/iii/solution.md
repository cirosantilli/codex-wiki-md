<h1 id="3/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The second coordinate after two iterations satisfies

$$
b_{i+2}=b_i\bmod b_{i+1}<\frac{b_i}{2}
$$

whenever those two divisions are needed, by the same [remainder](../../../../../../remainder.md) bound, now applied to $b_i>b_{i+1}>0$. Let $m=\lfloor\log_2 b\rfloor$. If the [Euclidean algorithm](../../../../../../euclidean-algorithm.md) has not already stopped after $2m$ iterations, then its positive second coordinate is at most $1$: for $m\ge1$,

$$
0<b_{2m}<\frac b{2^m}<2.
$$

For $m=0$ the original $b$ is already $1$. A second coordinate of $1$ requires just one more division. Consequently

$$
\boxed{n\le2\lfloor\log_2 b\rfloor+1,\qquad n=O(\log b)\text{ as }b\to\infty.}
$$

This removes dependence on the potentially much larger input $a$. It improves the scale $\log_2(ab)$ to one involving only the smaller input; the rounded numerical bound need not be smaller for every pair. One may always take the minimum of the bounds in (ii) and (iii).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
