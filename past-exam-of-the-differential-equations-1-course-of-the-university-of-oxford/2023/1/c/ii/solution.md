<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Existence was proved by [Picard iteration](../../../../../picard-iteration.md). If $y$ and $v$ are any two continuous solutions with the same $b\ne0$, the previous part makes both bounded by $2B$. Subtracting their [Volterra integral equations](../../../../../volterra-integral-equation.md) gives

$$
\|y-v\|_\infty\leq\frac{\|y\|_\infty+\|v\|_\infty}{C_1}\|y-v\|_\infty
\leq\gamma\|y-v\|_\infty.
$$

Since $\gamma<1$, this forces $y=v$.

For $b=0$, zero is a solution. On any finite interval $[0,T]$, another continuous solution has a finite bound $K_T=\max_{[0,T]}|y|$. Since $K(t,s)\leq1$, its [integral equation](../../../../../integral-equation.md) implies

$$
|y(t)|\leq K_T\int_0^t|y(s)|\,ds.
$$

The [Gronwall inequality](../../../../../gronwall-inequality.md) gives $y=0$ on every such interval. Hence

$$
\boxed{|b|<C_1/4\quad\Longrightarrow\quad\text{exactly one continuous solution on }[0,\infty).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Differential equations 1 course of the University of Oxford](../../../../../differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
