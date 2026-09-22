<h1 id="6d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put

$$
S_n=\sum_{k=0}^{\lfloor(n-1)/2\rfloor}
\binom{n-k-1}{k}.
$$

The initial values are $S_1=S_2=1$. Using Pascal's identity and the convention that an out-of-range binomial coefficient is zero,

$$
\begin{aligned}
S_{n+2}
&=\sum_{k\geq0}\binom{n+1-k}{k}\\
&=\sum_{k\geq0}\binom{n-k}{k}
+\sum_{k\geq1}\binom{n-k}{k-1}\\
&=S_{n+1}+S_n.
\end{aligned}
$$

Thus $(S_n)$ has the same initial values and [linear recurrence relation](../../../../../../linear-recurrence-relation.md) as the [Fibonacci numbers](../../../../../../fibonacci-number.md). [Mathematical induction](../../../../../../mathematical-induction.md) gives

$$
\boxed{
F_n=\sum_{k=0}^{\lfloor(n-1)/2\rfloor}
\binom{n-k-1}{k}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6D](../../6d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
