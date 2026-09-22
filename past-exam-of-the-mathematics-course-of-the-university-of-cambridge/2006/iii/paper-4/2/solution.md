<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [standard Young tableau](../../../../../standard-young-tableau.md) is a filling by $1,\ldots,n$, each used once, increasing along rows and down columns. A [semistandard Young tableau](../../../../../semistandard-young-tableau.md) is a filling by positive integers, weakly increasing along rows and strictly increasing down columns. Its content $\mu$ means that the entry $i$ occurs $\mu_i$ times. The [Kostka number](../../../../../kostka-number.md) $K_{\lambda\mu}$ counts [semistandard tableaux](../../../../../semistandard-young-tableau.md) of shape $\lambda$ and content $\mu$. The [dominance order on partitions](../../../../../dominance-order-on-partitions.md) is

$$
\lambda\unrhd\mu\quad\Longleftrightarrow\quad
\sum_{i\le r}\lambda_i\ge\sum_{i\le r}\mu_i\quad\text{for every }r.
$$

Strict dominance adds $\lambda\ne\mu$. The [Young permutation module](../../../../../young-permutation-module.md) is $M^\mu=F\{\mu\text{-tabloids}\}=\operatorname{Ind}_{S_{\mu_1}\times S_{\mu_2}\times\cdots}^{S_n}\mathbf1$.

Let $D^\lambda$ be a [composition factor](../../../../../composition-factor.md) of $M^\mu$. It occurs as a [submodule](../../../../../submodule.md) of some quotient $M^\mu/U$, so its defining surjection $S^\lambda\to D^\lambda$ gives a nonzero map $\theta:S^\lambda\to M^\mu/U$. With $t^*$ the row reversal from Question 1, $\kappa_te_{t^*}=he_t$, $h\ne0$, and the cyclic generator cannot have zero image under $\theta$. Therefore $\kappa_t$ acts nontrivially on $M^\mu/U$, and hence on $M^\mu$. The column-cancellation argument proves $\lambda\unrhd\mu$.

When $\lambda=\mu$, the identity $\kappa_tv=\langle v,e_t\rangle e_t$ shows more: the image of every nonzero map $S^\mu\to M^\mu/U$ is $(S^\mu+U)/U$. In a [composition series](../../../../../composition-series.md) of $M^\mu$, a factor isomorphic to $D^\mu$ can thus occur only at the step where $S^\mu$ first becomes contained in the series term. Once contained, every later such map would have zero image. Since the quotient $D^\mu$ of the [submodule](../../../../../submodule.md) $S^\mu$ certainly occurs when $\mu$ is regular, it occurs exactly once. If $\mu$ is not regular, no simple is indexed by $\mu$. Consequently **every other factor has a strictly dominating regular label**. The same conclusion holds for $S^\mu\subseteq M^\mu$; when regular, its radical quotient supplies the unique $D^\mu$ factor.

The integral standard-basis theorem says that the standard [polytabloids](../../../../../polytabloid.md) form a basis over every [field](../../../../../field.md). Thus $\dim S_F^\mu=f^\mu$ is independent of [characteristic](../../../../../characteristic-of-a-field.md). In the [decomposition matrix](../../../../../decomposition-matrix-modular-representation-theory.md), rows are indexed by all ordinary shapes $\mu$ and columns by regular shapes $\lambda$:

$$
d_{\mu\lambda}=[S_F^\mu:D_F^\lambda],\qquad
\boxed{d_{\mu\lambda}=0\text{ unless }\lambda\unrhd\mu,\quad d_{\lambda\lambda}=1.}
$$

Ordering shapes by a common linear extension of dominance gives a rectangular triangular matrix, whose regular-row square submatrix is unitriangular. The standard basis also gives $f^\mu=\sum_\lambda d_{\mu\lambda}\dim D^\lambda$.

[Young's rule](../../../../../young-s-rule.md) states that $M^\mu$ has a [Specht filtration](../../../../../specht-filtration.md) with $K_{\lambda\mu}$ copies of $S^\lambda$. In [characteristic](../../../../../characteristic-of-a-field.md) zero this is a direct-sum decomposition into [irreducibles](../../../../../irreducible-representation.md). In positive [characteristic](../../../../../characteristic-of-a-field.md) these are Specht factors, not simple factors; rather

$$
[M^\mu:D^\alpha]=\sum_\lambda K_{\lambda\mu}d_{\lambda\alpha}.
$$

For content $\lambda$ and shape $\lambda$, entries at most $r$ must lie in the first $r$ rows, because columns strictly increase. Their number is exactly the size of those rows, so successive rows must be filled by their row number. Hence $K_{\lambda\lambda}=1$. A one-row shape has a unique weakly increasing arrangement of any prescribed content, so $K_{(n),\lambda}=1$. Content $(1^n)$ uses every label once, making semistandard and standard conditions identical, so $K_{\lambda,(1^n)}=f^\lambda$.

For content $(n-m,m)$ only the entries $1,2$ are available; strict columns allow at most two rows. In shape $(n-j,j)$ every bottom entry is $2$ and every entry above it is $1$. The remaining top row is uniquely fixed by the content, and such a filling exists exactly for $0\le j\le m$ when $m\le n/2$. [Young's rule](../../../../../young-s-rule.md) therefore gives

$$
\boxed{[n-m][m]=\sum_{j=0}^m[n-j,j],}
$$

where multiplication denotes induction from the indicated [Young subgroup](../../../../../young-subgroup.md), not pointwise multiplication of [characters](../../../../../character-of-a-representation.md) of the same group. The [dimension](../../../../../dimension-vector-space.md) of this [permutation module](../../../../../permutation-module.md) is $\binom nm$. Subtracting the analogous identity with $m-1$ yields

$$
\boxed{\dim S^{(n-m,m)}=\binom nm-\binom n{m-1}
=\frac{n-2m+1}{n-m+1}\binom nm,}
$$

with $\binom n{-1}=0$ for $m=0$. This [dimension](../../../../../dimension-vector-space.md) holds over every [field](../../../../../field.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
