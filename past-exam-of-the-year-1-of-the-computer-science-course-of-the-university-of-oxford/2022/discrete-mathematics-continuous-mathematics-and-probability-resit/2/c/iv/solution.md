<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**True for every fixed $k\geq0$.** Extract $e^n$ from inside the [logarithm](../../../../../../logarithm.md):

$$
\log(e^n+n^k)-n=\log(1+n^ke^{-n}).
$$

Choose an [integer](../../../../../../integer-split.md) $m>k$. The nonnegative terms of the [exponential series](../../../../../../exponential-series.md) give $e^n\geq n^m/m!$ for $n>0$, whence

$$
0\leq n^ke^{-n}\leq m!n^{k-m}\longrightarrow0.
$$

Since $0\leq\log(1+u)\leq u$ for $u\geq0$, the displayed expression tends to zero and is therefore $O(1)$. The constant and cutoff may depend on the fixed $k$; no uniform assertion over unbounded $k$ is being made.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
