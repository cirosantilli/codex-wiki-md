<h1 id="27g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) states that if  
$0\leq f_n\uparrow f$ pointwise, then

$$
\int f_n\,d\mu\uparrow\int f\,d\mu,
$$

allowing the value $+\infty$.

Monotonicity of the integral shows that the increasing limit $L$ of the left side is at most $\int f$. Conversely, let $s$ be a nonnegative simple function with $s\leq f$, and fix $0<c<1$. The sets

$$
E_n=\{f_n\geq cs\}
$$

increase to the support of $s$. Hence

$$
\int f_n\,d\mu\geq c\int_{E_n}s\,d\mu
\longrightarrow c\int s\,d\mu.
$$

Let $c\uparrow1$ and take the supremum over all simple $s\leq f$. This gives  
$L\geq\int f$, proving equality.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27G](../../27g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
