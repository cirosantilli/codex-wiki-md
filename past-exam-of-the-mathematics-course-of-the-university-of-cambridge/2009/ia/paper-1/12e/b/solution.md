<h1 id="12e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $|f|\le M$. If $M=0$ the result is immediate, so take $M>0$. Given $\varepsilon>0$, choose $0<\delta<\varepsilon/(4M)$ and the finitely many intervals supplied by the hypothesis. On each $[a_i,b_i]$, choose a [partition of an interval](../../../../../../partition-of-an-interval.md) whose [Darboux sum](../../../../../../darboux-sum.md) gap is less than $\varepsilon/(2n)$, using [Riemann integrability](../../../../../../riemann-integrable-function.md) there.

Combine all these partitions with $0,1$ and all interval endpoints to obtain a global [partition of an interval](../../../../../../partition-of-an-interval.md) $P$. On the chosen intervals the gaps add to less than $\varepsilon/2$. The complementary intervals have total length

$$
1-\sum_{i=1}^n(b_i-a_i)\le\delta,
$$

and on each the difference between the supremum and infimum is at most $2M$. Consequently

$$
U(f,P)-L(f,P)<\frac\varepsilon2+2M\delta<\varepsilon.
$$

The [Riemann integrability criterion](../../../../../../riemann-integrability-criterion.md) proves **$f$ is [Riemann integrable](../../../../../../riemann-integrable-function.md) on $[0,1]$**. Shared endpoints cause no problem: the [Darboux sums](../../../../../../darboux-sum.md) use closed intervals, and the complementary interval estimate includes every endpoint value. This proves [Riemann integrability from almost full interval coverage](../../../../../../riemann-integrability-from-almost-full-interval-coverage.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12E](../../12e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
