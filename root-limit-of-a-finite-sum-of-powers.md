# Root limit of a finite sum of powers

↑ **Parent:** [Limit of a function](limit-of-a-function.md)

For finitely many fixed nonnegative [real numbers](real-number.md) $b_1,\ldots,b_m$, with $m\geq1$,

$$
\boxed{\lim_{p\to\infty}\left(\sum_{j=1}^m b_j^p\right)^{1/p}=\max_{1\leq j\leq m}b_j.}
$$

Let $M$ be that maximum. If $M=0$, every term is zero. Otherwise $M^p\leq\sum b_j^p\leq mM^p$ for $p>0$. Taking roots gives $M\leq(\sum b_j^p)^{1/p}\leq m^{1/p}M$, and $m^{1/p}\to1$. The [squeeze theorem](squeeze-theorem.md) proves the result, including ties between the largest bases. For example, $(1+a^p+(a^2/2)^p)^{1/p}$ tends to $\max(1,a,a^2/2)$ for $a\geq0$. The finiteness and fixed number of terms supply the upper factor $m$; an infinite [sum](sum.md) needs further hypotheses.

## ↑ Ancestors (7)

1. [Limit of a function](limit-of-a-function.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/19/d/iii/solution.md)
