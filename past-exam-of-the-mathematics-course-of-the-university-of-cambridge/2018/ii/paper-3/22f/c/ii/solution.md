<h1 id="22f/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Regard the set-theoretic inclusion

$$
I:L^q(X)\longrightarrow L^p(X)
$$

as a linear map between Banach spaces. Its graph is closed. Indeed, if $f_n\to f$ in $L^q$ and $f_n\to g$ in $L^p$, part (i) gives an almost-everywhere convergent subsequence for the first convergence and then a further subsequence converging almost everywhere for the second; hence $f=g$ almost everywhere. The [closed graph theorem](../../../../../../../closed-graph-theorem.md) therefore gives

$$
\lVert f\rVert_p\leq C\lVert f\rVert_q.
$$

Let $E_R=X\cap B(0,R)$. It has finite measure, and $\mu(E_R)\uparrow\mu(X)$. Applying the bound to $\mathbf1_{E_R}$ gives, for finite $q$,

$$
\mu(E_R)^{1/p}
\leq C\mu(E_R)^{1/q},
$$

so $\mu(E_R)^{1/p-1/q}\leq C$. For $q=\infty$, it gives $\mu(E_R)^{1/p}\leq C$. In either case the measures $\mu(E_R)$ are uniformly bounded. Continuity from below now yields

$$
\boxed{\mu(X)<\infty.}
$$

This proves the converse summarized by [Lq inclusion implies finite measure on a Euclidean Borel subset](../../../../../../../lq-inclusion-implies-finite-measure-on-a-euclidean-borel-subset.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [22F](../../../22f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
