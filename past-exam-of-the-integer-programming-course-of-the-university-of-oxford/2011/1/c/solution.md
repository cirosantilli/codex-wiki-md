<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On a finite [ground set](../../../../ground-set.md) $E$, a **[submodular rank function](../../../../submodular-rank-function.md)** is a [set function](../../../../set-function.md) $r:2^E\to\mathbb R$ with the following properties:

$$
\begin{aligned}
&r(\varnothing)=0,\\
&A\subseteq B\Longrightarrow r(A)\leq r(B),\\
&r(A)+r(B)\geq r(A\cup B)+r(A\cap B),\\
&r(A\cup\{e\})-r(A)\in\{0,1\}\quad(e\notin A).
\end{aligned}
$$

These are normalization, monotonicity, [submodularity](../../../../submodular-set-function.md), and unit [integer](../../../../integer-split.md) increments. In particular its values are nonnegative [integers](../../../../integer-split.md) with $r(A)\leq|A|$. Equivalently, one can require an integer-valued normalized monotone submodular function with $r(\{e\})\leq1$: diminishing returns then bounds every marginal increment by one. A general real-valued submodular function need not be a [matroid](../../../../matroid.md) rank.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
