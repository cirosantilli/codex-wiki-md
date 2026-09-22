# Growing-clique overlap bound

↑ **Parent:** [Overlap formula for the variance of a clique count](overlap-formula-for-the-variance-of-a-clique-count.md)

Write $\mu_r=\binom nrp^{\binom r2}$ and $T_s=\binom rs\binom{n-r}{r-s}p^{-\binom s2}/\binom nr$. The first mean condition implies $p^{-1}\leq(en/r)^{2/(r-1)}$ eventually. For $2\leq s\leq r/2$, this yields $T_s\leq(C/s)^s$, and each fixed-$s$ term tends to zero when $n\geq r^3$. The second mean condition implies $p\leq((r+1)/n)^{2/r}$ eventually. Writing $s=r-j$ gives $T_{r-j}=\mu_r^{-1}\binom rj\binom{n-r}j p^{j(2r-j-1)/2}\leq\mu_r^{-1}(C/j)^j$ for $1\leq j\leq r/2$, and $T_r=\mu_r^{-1}$. Both bounding series are summable. The [overlap formula for the variance of a clique count](overlap-formula-for-the-variance-of-a-clique-count.md) therefore gives relative variance tending to zero; the [second moment method](second-moment-method.md) proves an $r$-[clique](clique-graph-theory.md) exists [with high probability](with-high-probability.md).

## ↑ Ancestors (8)

1. [Overlap formula for the variance of a clique count](overlap-formula-for-the-variance-of-a-clique-count.md)
2. [Clique count in a binomial random graph](clique-count-in-a-binomial-random-graph.md)
3. [Binomial random graph](binomial-random-graph.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/1/ii/solution.md)
