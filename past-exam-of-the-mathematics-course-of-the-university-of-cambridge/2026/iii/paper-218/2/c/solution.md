<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N_\delta$ count sample points in the intersection of $[0,1]^d$ with the $\ell^\infty$ ball of radius $\delta$ around $x$. That intersection has volume at least $\delta^d$, so $N_\delta\sim\operatorname{Bin}(n,q)$ with $q\geq M\delta^d$. The event $\lVert X_{(L)}-x\rVert_\infty>\delta$ implies $N_\delta<L$. Since $\operatorname{Var}(N_\delta)\leq nq$ and $nq\geq nM\delta^d\geq L$, [Chebyshev inequality](../../../../../../chebyshev-inequality.md) gives

$$
\mathbb P(N_\delta<L)
\leq\frac{nq}{(nq-L)^2}
\leq\frac{nM\delta^d}{(nM\delta^d-L)^2}.
$$

Taking the minimum with the trivial bound one proves the result.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
