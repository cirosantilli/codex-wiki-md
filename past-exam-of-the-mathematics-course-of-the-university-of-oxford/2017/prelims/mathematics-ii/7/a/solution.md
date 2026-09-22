<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By the [Heine-Cantor theorem](../../../../../../heine-cantor-theorem.md), a [continuous function](../../../../../../continuous-function.md) on the [compact interval](../../../../../../compact-interval.md) $[a,b]$ is [uniformly continuous](../../../../../../uniform-continuity.md). Given $\varepsilon>0$, choose $\delta>0$ such that $|f(s)-f(t)|<\varepsilon$ whenever $s,t\in[a,b]$ and $|s-t|<\delta$.

Choose a finite [partition of an interval](../../../../../../partition-of-an-interval.md) $a=t_0<t_1<\cdots<t_m=b$ with every width below $\delta$. Define the [step function](../../../../../../step-function.md)

$$
\phi(t)=f(t_{j-1})\quad(t_{j-1}\leq t<t_j),\qquad\phi(b)=f(b).
$$

For each $t<b$, its distance from the chosen left endpoint is below $\delta$, so $|f(t)-\phi(t)|<\varepsilon$; at $b$ the error is zero. Hence

$$
\boxed{|f(t)-\phi(t)|<\varepsilon\quad\text{for every }t\in[a,b].}
$$

A [step function](../../../../../../step-function.md) may have separately assigned values at its finitely many partition points; these values do not affect its [Riemann integral](../../../../../../riemann-integral.md). If $a=b$, simply take $\phi=f$ on that singleton.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
