<h1 id="5e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove both identities by [mathematical induction](../../../../../../mathematical-induction.md). They hold at $n=1$. Assume they hold at $n$. Using $F_{n-1}=F_{n+1}-F_n$,

$$
\begin{aligned}
F_{2n+2}&=F_{2n+1}+F_{2n}\\
&=F_n^2+F_{n+1}^2+F_n(F_{n-1}+F_{n+1})\\
&=F_{n+1}(F_n+F_{n+2}).
\end{aligned}
$$

Adding this to $F_{2n+1}=F_n^2+F_{n+1}^2$ and using $F_{n+2}=F_n+F_{n+1}$ gives

$$
F_{2n+3}=F_{n+1}^2+F_{n+2}^2.
$$

These are precisely the two assertions with $n$ replaced by $n+1$, completing the induction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
