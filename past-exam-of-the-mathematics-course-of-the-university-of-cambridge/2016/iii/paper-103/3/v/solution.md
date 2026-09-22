<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use the tableau representation supplied by [Young seminormal form](../../../../../../young-seminormal-form.md), stated explicitly in Question 5, or its normalized [Young orthogonal form](../../../../../../young-orthogonal-form.md). It constructs the complex [Specht module](../../../../../../specht-module.md) $S^\lambda$ with one basis vector for each [standard Young tableau](../../../../../../standard-young-tableau.md) of shape $\lambda$. Its adjacent-transposition matrices imply the content [eigenvalues](../../../../../../eigenvalue.md) directly.

Indeed, start with $X_1=0$ and use $X_{i+1}=s_iX_is_i+s_i$. On an admissible pair $T,R=s_iT$, set $a=c_T(i)$, $b=c_T(i+1)$, $d=b-a$, and $q=\sqrt{1-d^{-2}}$. In the orthogonal basis, $X_i$ is $\operatorname{diag}(a,b)$ and

$$
s_i=\begin{pmatrix}d^{-1}&q\\q&-d^{-1}\end{pmatrix}.
$$

Multiplication gives

$$
s_i\begin{pmatrix}a&0\\0&b\end{pmatrix}s_i+s_i
=\begin{pmatrix}b&0\\0&a\end{pmatrix}.
$$

For a nonadmissible swap, $s_i=\pm1$ and the next content differs by the same $\pm1$, giving the same conclusion. Induction therefore proves $X_iw_T=c_T(i)w_T$. Every [content vector of a standard Young tableau](../../../../../../content-vector-of-a-standard-young-tableau.md), reconstructed as a [standard Young tableau](../../../../../../standard-young-tableau.md) in part (iv), is consequently a spectral weight. Together with the reverse inclusion,

$$
\boxed{\operatorname{Spec}(n)=\operatorname{Cont}(n)}.
$$

An admissible adjacent swap has nonzero off-diagonal coefficient in [Young orthogonal form](../../../../../../young-orthogonal-form.md), and the local spectral calculation in part (i) keeps it inside one [irreducible representation](../../../../../../irreducible-representation.md). Thus $\alpha\approx\beta$ implies $\alpha\sim\beta$.

Two [standard Young tableaux](../../../../../../standard-young-tableau.md) of one shape are connected by admissible swaps. Regard each as a [linear extension of a partially ordered set](../../../../../../linear-extension.md) of cells. Move the first cell of the desired extension to the front of the other extension: every cell it crosses is incomparable with it, since otherwise their order would be forced in both extensions. Repeat after fixing that first cell. Each step swaps consecutive labels in incomparable cells. Such cells lie strictly northeast and southwest of each other, so their contents differ by at least $2$ in absolute value. These are exactly admissible swaps.

This also establishes irreducibility of the constructed tableau representations. A submodule is invariant under the commuting $X_j$ and hence under their joint spectral projections; since their weights are distinct, it is a sum of tableau lines. A nonzero off-diagonal coefficient propagates any included line along every admissible edge, and connectivity then includes all lines. Different shapes give nonisomorphic modules, since their content-vector sets are disjoint and content reconstruction determines the shape. Finally, the [Robinson–Schensted correspondence](../../../../../../robinson-schensted-correspondence.md) gives $\sum_{\lambda\vdash n}f_\lambda^2=n!$, and the [sum of squares of irreducible degrees](../../../../../../sum-of-squares-of-irreducible-degrees.md) leaves room for no other [irreducible representations](../../../../../../irreducible-representation.md).

Thus within each [irreducible module](../../../../../../irreducible-module.md) the weights are exactly the tableaux of one shape, so $\alpha\sim\beta$ implies $\alpha\approx\beta$. Hence **the two equivalence relations coincide**.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
