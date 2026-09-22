<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [distribution function](../../../../../../cumulative-distribution-function.md) is nondecreasing and right-continuous. Every nondecreasing function has finite left limits, so $F$ is [càdlàg](../../../../../../cadlag.md). Along each partition its increments are nonnegative and telescope, giving

$$
V_F(t)=F(t)-F(0).
$$

For each $n$, the set $A^{(n)}=\{s\in[0,n]:\Delta F(s)\geq2^{-n}\}$ is finite because the sum of its positive jumps is at most $F(n)-F(0)$. Every jump belongs to some $A^{(n)}$, so $A_F=\bigcup_nA^{(n)}$ is countable.

For a finite partition, the identity $y^2-x^2=2y(y-x)-(y-x)^2$ gives

$$
F(t)^2-F(0)^2
=2\sum_kF(t\wedge t_k^n)\bigl(F(t\wedge t_k^n)-F(t\wedge t_{k-1}^n)\bigr)
-\sum_k\bigl(F(t\wedge t_k^n)-F(t\wedge t_{k-1}^n)\bigr)^2.
$$

The first sum tends to the [Lebesgue-Stieltjes integral](../../../../../../lebesgue-stieltjes-integration.md) $2\int_0^tF\,dF$. In the second, intervals containing no prescribed large jump contribute at most their largest increment times $F(t)-F(0)$; first retain finitely many jumps above a threshold and then let the threshold vanish. The limit is therefore $\sum_{s\in A_F\cap(0,t]}|\Delta F(s)|^2$, proving

$$
\boxed{F(t)^2=F(0)^2+2\int_0^tF\,dF-
\sum_{s\in A_F\cap(0,t]}|\Delta F(s)|^2.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
