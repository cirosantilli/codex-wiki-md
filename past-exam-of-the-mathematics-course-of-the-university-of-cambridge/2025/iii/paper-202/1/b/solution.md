<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Refine a dyadic partition by inserting $s$ and $t$. The [triangle inequality](../../../../../../triangle-inequality.md) shows that its variation over $[s,t]$ is at least $|f(t)-f(s)|$. Passing to the defining limit gives

$$
V_f(t)-V_f(s)\geq|f(t)-f(s)|.
$$

Consequently the càdlàg functions

$$
F=\frac{V_f+f}{2},\qquad G=\frac{V_f-f}{2}
$$

are nondecreasing: for $s\leq t$, the displayed inequality makes both increments nonnegative. Thus they are distribution functions in the Stieltjes sense and $f=F-G$; this is the [Jordan decomposition of a function of bounded variation](../../../../../../jordan-decomposition-of-a-function-of-bounded-variation.md).

Now $A_f\subseteq A_F\cup A_G$, so $A_f$ is countable by part (a). For any finite subset $J\subseteq A_f\cap(0,t]$, partitions isolating its points and the triangle inequality give

$$
\sum_{s\in J}|\Delta f(s)|\leq V_f(t).
$$

Taking the supremum over finite $J$ proves $\sum_{s\in A_f\cap(0,t]}|\Delta f(s)|<\infty$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
