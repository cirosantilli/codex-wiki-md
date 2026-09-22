<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

[Rouché's theorem](../../../../../rouche-s-theorem.md) states that if $f,g$ are holomorphic on a neighborhood of a closed disc with boundary $C$ and $|g|<|f|$ on $C$, then $f$ and $f+g$ have the same number of zeros in the disc, counted with multiplicity. More generally the conclusion holds for a simple closed contour whose interior lies in their domain. To prove it, set $f_t=f+tg$ for $0\le t\le1$. The strict boundary inequality ensures $f_t\ne0$ on $C$. By the [argument principle](../../../../../argument-principle.md),

$$
N(t)=\frac1{2\pi i}\int_C\frac{f_t'(z)}{f_t(z)}dz
$$

is the integer number of zeros inside. The integrand is continuous in $t$ uniformly on $C$, since its denominator is bounded away from zero on the compact product $C\times[0,1]$. Thus $N(t)$ is continuous and integer-valued, so constant. This proves the theorem.

On $|z|=1$, the term $8z^6$ dominates the remaining terms because $3+1+2+1=7<8$. Thus the polynomial has six zeros inside the unit circle. On $|z|=2$, $3z^9$ dominates because its modulus is $1536$, whereas the sum of the other bounds is $512+32+16+1=561$. There are therefore nine zeros inside radius two. The strict inequalities exclude boundary zeros, so

$$
\boxed{9-6=3\text{ zeros lie in }1<|z|<2,\text{ counted with multiplicity}.}
$$

For the [fixed-degree polynomial limit](../../../../../fixed-degree-polynomial-limit.md), choose $d+1$ distinct complex nodes $\zeta_0,\ldots,\zeta_d$. Write $p_n(z)=\sum_{j=0}^da_{j,n}z^j$, inserting zero coefficients if necessary. The vector of values at the nodes equals the fixed [Vandermonde matrix](../../../../../vandermonde-matrix.md) times the coefficient vector. Its determinant is $\prod_{i<j}(\zeta_j-\zeta_i)\ne0$. Convergence of the values therefore implies coefficient convergence, say $a_{j,n}\to a_j$. For $p(z)=\sum_{j=0}^da_jz^j$ and a compact set with $|z|\le R$,

$$
\sup|p_n(z)-p(z)|\le\sum_{j=0}^d|a_{j,n}-a_j|R^j\longrightarrow0.
$$

This proves that the given limit is a [polynomial](../../../../../polynomial-split.md) of degree at most $d$ without invoking any theorem about uniform limits of holomorphic functions.

When the limit has $d$ distinct roots, choose pairwise disjoint small closed discs around them, with no limit root on their boundaries. On each boundary $|p|$ has a positive minimum. Uniform convergence makes $|p_n-p|<|p|$ there for all sufficiently large $n$, so [Rouché's theorem](../../../../../rouche-s-theorem.md) puts exactly one root $z_{i,n}$ of $p_n$ in each disc. For every smaller disc about $z_i$ the same argument applies eventually. The unique root in the original disc must then lie in the smaller one, proving

$$
\boxed{z_{i,n}\longrightarrow z_i\quad\text{for each }i,\text{ with roots defined for all sufficiently large }n.}
$$

The literal demand for a root at every initial index needs this finite-index qualification: $p_1=1$, $p_n=z$ for $n\ge2$ satisfies the hypotheses with limit $z$, but $p_1$ has no root. If every initial polynomial has a root, arbitrary choices at the finitely many exceptional indices extend the convergent sequences; otherwise the sequences necessarily start at an eventual index.

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
