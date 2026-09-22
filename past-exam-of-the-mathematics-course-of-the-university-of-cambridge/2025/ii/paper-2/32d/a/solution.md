<h1 id="32d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Integration by parts gives the recurrence

$$
\gamma(x,y)=y^{x-1}e^{-y}+(x-1)\gamma(x-1,y).
$$

Iterating $N$ times yields

$$
\gamma(x,y)=y^{x-1}e^{-y}
\sum_{n=0}^{N-1}(x-1)(x-2)\cdots(x-n)y^{-n}
+R_N,
$$

where the empty product for $n=0$ is one and

$$
R_N=(x-1)(x-2)\cdots(x-N)\gamma(x-N,y).
$$

For fixed $x$, the remainder has the order of the first omitted term as $y\to\infty$. Therefore

$$
\boxed{a_0(x)=1,\qquad
a_n(x)=\prod_{j=1}^n(x-j)\quad(n\geq1).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32D](../../32d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
