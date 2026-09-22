<h1 id="22h/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose first that $\|x_n-x_\infty\|\to0$. The reverse [triangle inequality](../../../../../../../triangle-inequality.md) gives

$$
\big|\|x_n\|-\|x_\infty\|\big|
\leq\|x_n-x_\infty\|\longrightarrow0,
$$

so (i) implies (ii).

It also implies (iii). Given $\epsilon>0$, choose $N$ so that

$$
\|x_n-x_\infty\|^2<\frac\epsilon8
\qquad(n\geq N).
$$

By the [Parseval identity for a Hilbertian basis](../../../../../../../parseval-identity-for-a-hilbertian-basis.md), choose $I_0$ so that the basis tail of $x_\infty$ beyond $I_0$ is less than $\epsilon/8$. For $n\geq N$ and $I\geq I_0$,

$$
\sum_{i\geq I}|\langle x_n,e_i\rangle|^2
\leq
2\|x_n-x_\infty\|^2
+2\sum_{i\geq I}|\langle x_\infty,e_i\rangle|^2
<\frac\epsilon2.
$$

There are only finitely many $n<N$, so increasing $I$ makes each of their tails less than $\epsilon$. Thus one $I$ works for every $n$, proving (iii).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [22H](../../../22h.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
