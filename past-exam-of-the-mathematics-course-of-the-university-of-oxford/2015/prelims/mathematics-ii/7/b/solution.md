<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $G=\int_a^bg(t)\,dt\geq0$ and $I=\int_a^bf(t)g(t)\,dt$. By the [extreme value theorem](../../../../../../extreme-value-theorem.md), $f$ attains a [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md) $m$ and a [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) $M$ on $[a,b]$. Because $g\geq0$, the [monotonicity of the Riemann integral](../../../../../../monotonicity-of-the-riemann-integral.md) gives

$$
mG\leq I\leq MG.
$$

If $G=0$, this forces $I=0$, and every $c\in[a,b]$ satisfies the required identity. This includes $a=b$.

If $G>0$, divide to obtain $m\leq I/G\leq M$. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md), applied between points where the [continuous function](../../../../../../continuous-function.md) $f$ attains $m$ and $M$, supplies $c\in[a,b]$ with $f(c)=I/G$. Hence the [weighted mean value theorem for integrals](../../../../../../weighted-mean-value-theorem-for-integrals.md) gives

$$
\boxed{\int_a^bf(t)g(t)\,dt=f(c)\int_a^bg(t)\,dt.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
