<h1 id="m/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With probability $2/3$, the chain starts at $+1$ and $T=1$. Conditional on starting at $-1$, it takes a geometric number $G$ of transitions to first reach $+1$, with success probability $1-p$, so $T=1+G$. The [probability generating function](../../../../../probability-generating-function.md) is therefore

$$
\boxed{\mathbb E[s^T]=\frac23s+\frac13s\frac{(1-p)s}{1-ps}
=\frac23s+\frac{(1-p)s^2}{3(1-ps)}.}
$$

The parameter $q$ is absent because the process stops at its first visit to $+1$. At $s=1$ the expression equals one, confirming eventual hitting with probability one.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [M](../../../m.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
