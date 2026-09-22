<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [uniform pro-p group](../../../../../../uniform-pro-p-group.md) is a finitely generated [powerful pro-p group](../../../../../../powerful-pro-p-group.md) whose [lower p-series](../../../../../../lower-p-series.md) $P_1=G$, $P_{i+1}=\overline{P_i^p[P_i,G]}$ has constant successive indices. For odd $p$, the [powerful pro-p group](../../../../../../powerful-pro-p-group.md) condition means $[G,G]\subseteq G^p$, with closed generated powers understood. For $p=2$ it means $[G,G]\subseteq G^4$. For finitely generated [powerful pro-p groups](../../../../../../powerful-pro-p-group.md), uniformity is equivalent to being a [torsion-free group](../../../../../../torsion-free-group.md).

It is convenient to use general [matrix](../../../../../../matrix.md) size $d$, then put $d=p$. Let $U_m=1+p^mM_d(\mathbb Z_p)$. The required [kernel](../../../../../../kernel-of-a-linear-map.md) is $U_1$, the [inverse limit](../../../../../../inverse-limit.md) of its finite p-group quotients. For odd $p$, the convergent [matrix logarithm](../../../../../../matrix-logarithm.md) and [matrix exponential](../../../../../../matrix-exponential.md) series

$$
\log(1+A)=\sum_{r\ge1}\frac{(-1)^{r+1}A^r}{r},\qquad\exp(B)=\sum_{r\ge0}\frac{B^r}{r!}
$$

are inverse maps between $U_m$ and $p^mM_d(\mathbb Z_p)$. The valuation bounds for $A,B\in pM_d$ ensure convergence and integrality. They give $\log(u^p)=p\log u$ and hence a bijective power map $U_m\to U_{m+1}$: the unique root of $v\in U_{m+1}$ is $\exp(p^{-1}\log v)$.

Direct [matrix](../../../../../../matrix.md) multiplication gives $[U_i,U_j]\subseteq U_{i+j}$, so $[U_1,U_1]\subseteq U_2=U_1^p$ and it is a [powerful pro-p group](../../../../../../powerful-pro-p-group.md). Moreover

$$
U_m/U_{m+1}\cong(M_d(\mathbb F_p),+),\qquad\boxed{[U_m:U_{m+1}]=p^{d^2}}.
$$

The $d^2$ elements $1+pE_{ij}$ topologically generate: their $p^{m-1}$th powers give all [matrix](../../../../../../matrix.md) [basis](../../../../../../basis.md) directions in $U_m/U_{m+1}$, since $(1+pE_{ij})^{p^{m-1}}\equiv1+p^mE_{ij}\pmod{p^{m+1}}$. Successive correction of each [matrix](../../../../../../matrix.md) entry, followed by completeness, approximates every element by words in these generators.

Its [lower p-series](../../../../../../lower-p-series.md) is exactly $U_m$ and the indices are constant; thus the [group](../../../../../../group-split.md) is a [uniform pro-p group](../../../../../../uniform-pro-p-group.md). Alternatively, the logarithm excludes nontrivial p-power torsion. Setting $d=p$ gives **a [uniform pro-p group](../../../../../../uniform-pro-p-group.md) [kernel](../../../../../../kernel-of-a-linear-map.md) of dimension and generator number $p^2$**, with indices $p^{p^2}$. This is the [odd-prime principal p-adic congruence subgroup is uniform](../../../../../../odd-prime-principal-p-adic-congruence-subgroup-is-uniform.md) result. The odd-prime condition matters: $-I$ is nontrivial order-two torsion in $1+2M_d(\mathbb Z_2)$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
