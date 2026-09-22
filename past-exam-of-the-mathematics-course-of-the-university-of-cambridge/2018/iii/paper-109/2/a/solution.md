<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Encode each point $x\in X$ by a partial [binary sequence](../../../../../../bitstream.md) of length $m$: coordinate $i$ is fixed to zero if $x\in A_i$, fixed to one if $x\in B_i$, and unrestricted otherwise. Disjointness makes these prescriptions consistent. Let $d(x)$ be the number of fixed coordinates, equivalently the number of pairs containing $x$, and let $S_x\subseteq\{0,1\}^m$ be the set of complete sequences consistent with them. Then $|S_x|=2^{m-d(x)}$.

The [separating family of disjoint set pairs](../../../../../../separating-family-of-disjoint-set-pairs.md) ensures that $S_x$ and $S_y$ are disjoint whenever $x\ne y$: one coordinate prescribes opposite bits. Counting the sequences in these disjoint subcubes gives the [disjoint subcube packing inequality](../../../../../../disjoint-subcube-packing-inequality.md)

$$
\sum_{x\in X}2^{-d(x)}\leq1.
$$

Since $z\mapsto2^{-z}$ is a [convex function](../../../../../../convex-function.md), [Jensen inequality](../../../../../../jensen-s-inequality.md) implies

$$
n\,2^{-\bar d}\leq\sum_{x\in X}2^{-d(x)}\leq1,
\qquad
\bar d=\frac1n\sum_xd(x)=\frac1n\sum_i(|A_i|+|B_i|)\leq\lambda m.
$$

Taking logarithms yields $\log_2n\leq\bar d\leq\lambda m$. Therefore, for $\lambda>0$,

$$
\boxed{m\geq\left\lceil\frac{\log_2 n}{\lambda}\right\rceil.}
$$

The PDF omits the qualification $\lambda>0$. For $n\geq2$, it follows from feasibility: separation requires positive total incidence, so the stated incidence bound cannot hold with $\lambda\leq0$. For $n=1$, separation is vacuous, and $\lambda=0$ makes the printed quotient undefined; the intended parameter range is $0<\lambda\leq1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
