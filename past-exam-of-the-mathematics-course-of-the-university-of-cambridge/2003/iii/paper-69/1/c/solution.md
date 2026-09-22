<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $m$ and take $n\ge m$. Comparing the two products defining $f_{nm}$ and the [monomial](../../../../../../monomial.md) $g_m(x)=x^m$, change one factor at a time. Every factor has absolute value at most one on $[0,1]$, so the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\|f_{nm}-g_m\|_\infty\le\sum_{r=0}^{m-1}\frac rn=\frac{m(m-1)}{2n},\qquad |f_{nm}(1)-1|\le\frac{m(m-1)}{2n}.
$$

The contraction proved in (a) and the [Bernstein falling-factorial identity](../../../../../../bernstein-falling-factorial-identity.md) from (b) now give

$$
\begin{aligned}
\|B_ng_m-g_m\|_\infty&\le\|B_n(g_m-f_{nm})\|_\infty+\|(f_{nm}(1)-1)g_m\|_\infty\\
&\le\boxed{\frac{m(m-1)}n\longrightarrow0}.
\end{aligned}
$$

This proves [uniform convergence](../../../../../../uniform-convergence.md) for each fixed [monomial](../../../../../../monomial.md); [linearity](../../../../../../linearity.md) then gives it for every fixed [polynomial](../../../../../../polynomial-split.md). The cases $m=0,1$ have zero error for every $n$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
