<h1 id="27h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) states that if $f_n$ are nonnegative measurable functions with $f_n(x)\uparrow f(x)$ almost everywhere, then

$$
\int f_n\,d\mu\uparrow\int f\,d\mu,
$$

where either side may be infinite.

The integrals increase and are bounded above by $\int f$, so let their limit be $L\leq\int f$. Let $s$ be a nonnegative simple function with $s\leq f$, and fix $0<c<1$. The sets

$$
E_n=\{x:f_n(x)\geq c s(x)\}
$$

increase and cover $\{s>0\}$ up to a null set. Hence continuity of measure from below gives

$$
\int f_n\,d\mu
\geq c\int_{E_n}s\,d\mu
\longrightarrow c\int s\,d\mu.
$$

**Thus $L\geq c\int s$. Taking the supremum over all simple $s\leq f$ and then letting $c\uparrow1$ gives $L\geq\int f$. Therefore equality holds.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27H](../../27h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
