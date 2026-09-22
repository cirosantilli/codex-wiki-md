<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Part i makes $K'_\varepsilon$ a closed subset of the compact metrizable space $K$, so it is compact metrizable and therefore separable. Choose the stated dense sequence $(f_m)$ and, using part iii, the sequences $(g_{m,n})$ and $(y_{m,n})$. In constructing the universal weakly null sequence $(z_n)$ from part b, retain a tail of each $y_m$ and write $z_{j(m,n)}=y_{m,n}$ along the retained subsequence, where $j(m,n)\to\infty$.

Each

$$
A_N=\bigcap_{n\geq N}\{f\in K:|f(z_n)|\leq\varepsilon/20\}
$$

is weak-star closed. Since $z_n\rightharpoonup0$, every fixed $f\in K$ belongs to some $A_N$, so $K=\bigcup_NA_N$. The compact Hausdorff space $K$ is a [Baire space](../../../../../../../baire-space.md), and the [Baire category theorem](../../../../../../../baire-category-theorem.md) implies that some $A_N$ has nonempty relative weak-star interior.

Suppose $K'_\varepsilon=K$. Choose a nonempty relatively open $O\subseteq A_N$ and then $f_m\in O$ by density. Since $g_{m,n}\xrightarrow{w^*}f_m$, eventually $g_{m,n}\in O$. For a sufficiently late retained index, also $j(m,n)\geq N$, and hence

$$
|g_{m,n}(y_{m,n})|
=|g_{m,n}(z_{j(m,n)})|
\leq\varepsilon/20,
$$

contradicting $|g_{m,n}(y_{m,n})|>\varepsilon/16$. Therefore the [One-step Szlenk derivation for a separable dual](../../../../../../../one-step-szlenk-derivation-for-a-separable-dual.md) gives $K'_\varepsilon\subsetneq K$ whenever $K$ is nonempty.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 106](../../../../paper-106-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
