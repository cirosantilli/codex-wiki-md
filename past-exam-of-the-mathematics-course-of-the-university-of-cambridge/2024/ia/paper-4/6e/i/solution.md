<h1 id="6e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $n=1$,

$$
F_2F_0-F_1^2=-1=(-1)^1.
$$

If $C_n=F_{n+1}F_{n-1}-F_n^2$, then the recurrence gives

$$
\begin{aligned}
C_{n+1}
&=F_{n+2}F_n-F_{n+1}^2\\
&=(F_{n+1}+F_n)F_n-F_{n+1}^2\\
&=F_n^2-F_{n+1}F_{n-1}=-C_n.
\end{aligned}
$$

Induction yields the [Fibonacci determinant identity](../../../../../../fibonacci-determinant-identity.md) known as Cassini's identity:

$$
\boxed{F_{n+1}F_{n-1}-F_n^2=(-1)^n}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
