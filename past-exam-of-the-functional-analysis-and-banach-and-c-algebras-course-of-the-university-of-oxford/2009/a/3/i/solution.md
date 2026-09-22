<h1 id="a/3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Baire category theorem](../../../../../baire-category-theorem.md) says that a nonempty [complete metric space](../../../../../complete-metric-space.md) is not a countable union of closed sets with empty interior; equivalently, every countable intersection of open dense sets is dense. To prove the latter, start with any nonempty open set $V$ and open dense sets $G_n$. Choose closed balls of positive radii with

$$
\overline B_1\subset V\cap G_1,\qquad\overline B_{n+1}\subset B_n\cap G_{n+1},\qquad r_n<2^{-n}.
$$

Each choice is possible by density and openness. Their centers form a [Cauchy sequence](../../../../../cauchy-sequence.md); its limit exists by completeness and belongs to every closed ball, hence to $V\cap\bigcap G_n$. This proves density and the theorem.

The [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) says that a pointwise bounded family $\mathcal T$ of bounded linear maps from a [Banach space](../../../../../banach-space-split.md) $X$ to a [normed space](../../../../../normed-vector-space-split.md) $Z$ has uniformly bounded operator norms. Put $E_m=\{x:\sup_{T\in\mathcal T}\|Tx\|\leq m\}$. These sets are closed and cover $X$. Baire gives an open ball $B(x_0,r)\subset E_m$. For $\|h\|<r$, the [triangle inequality](../../../../../triangle-inequality.md) applied to $T(x_0+h)-Tx_0$ gives $\|Th\|\leq2m$. Taking $h=(r/2)u$ for unit $u$ proves $\sup_T\|T\|\leq4m/r$.

For the particular expansion, uniqueness makes all coefficient maps and partial-sum maps linear. Since $P_kx\to x$, the norms $\|P_kx\|$ form a bounded sequence with limit $\|x\|$. Also, with $P_0=0$,

$$
|\varphi_n(x)|=\|\varphi_n(x)x_n\|=\|(P_n-P_{n-1})x\|\leq2\sup_k\|P_kx\|.
$$

This proves both preliminary bounds. The supremum therefore defines a finite [norm](../../../../../norm.md) $\|\cdot\|'$, with $\|x\|\leq\|x\|'$.

To prove **(i) implies (ii)**, the identity map from $(X,\|\cdot\|')$ to $(X,\|\cdot\|)$ is a bounded linear bijection. If (i) holds both spaces are Banach, so the [bounded inverse theorem](../../../../../bounded-inverse-theorem.md) makes its inverse bounded: $\|x\|'\leq C\|x\|$. This is precisely (ii).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
