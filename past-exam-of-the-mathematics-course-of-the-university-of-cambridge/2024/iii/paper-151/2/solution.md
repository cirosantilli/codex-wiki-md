<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Schur multiplier](../../../../../schur-multiplier.md) of a [group](../../../../../group-split.md) $G$ is

$$
M(G)=H_2(G,\mathbb Z),
$$

the second [group homology](../../../../../group-homology.md) group with trivial integral coefficients. If $G\cong F/R$ is a [free presentation](../../../../../free-presentation.md), [Hopf's formula](../../../../../hopf-s-formula.md) states that

$$
M(G)\cong\frac{R\cap[F,F]}{[F,R]}.
$$

Write $I_F=\ker(\mathbb ZF\to\mathbb Z)$ for the [augmentation ideal](../../../../../augmentation-ideal.md). The [presentation relation sequence](../../../../../presentation-relation-sequence.md) is

$$
0\longrightarrow R/[R,R]
\longrightarrow\mathbb ZG\otimes_{\mathbb ZF}I_F
\longrightarrow\mathbb ZG
\longrightarrow\mathbb Z\longrightarrow0,
$$

where $r[R,R]\mapsto1\otimes(r-1)$. If $F$ is free on a set $S$, then $I_F$ is free as a left $\mathbb ZF$-module on the elements $s-1$, so the two modules immediately preceding $\mathbb Z$ are free $\mathbb ZG$-modules. Resolving the [relation module](../../../../../relation-module.md) $R/[R,R]$ by free modules and splicing produces a [free resolution](../../../../../free-resolution.md) of $\mathbb Z$.

Apply the right-exact functor $\mathbb Z\otimes_{\mathbb ZG}-$ to this partial resolution. Its degree-two [homology](../../../../../homology-split.md) is the kernel of

$$
(R/[R,R])_G\longrightarrow
\left(\mathbb ZG\otimes_{\mathbb ZF}I_F\right)_G.
$$

The [coinvariant module](../../../../../coinvariant-module.md) on the left is $R/[F,R]$. On the right, the map $f-1\mapsto f[F,F]$ identifies the coinvariants with the [abelianization](../../../../../abelianization.md) $F/[F,F]$. The displayed map is induced by the inclusion $R\hookrightarrow F$, so its kernel is

$$
\ker\left(R/[F,R]\longrightarrow F/[F,F]\right)
=\frac{R\cap[F,F]}{[F,R]}.
$$

This proves [Hopf's formula](../../../../../hopf-s-formula.md).

For an [abelian group](../../../../../abelian-group.md) $A$, the [Schur multiplier of an abelian group](../../../../../schur-multiplier-of-an-abelian-group.md) is $M(A)\cong\bigwedge^2A$. One way to see the direct-sum rule is the degree-two [Künneth theorem](../../../../../kunneth-theorem.md):

$$
H_2(A\times B,\mathbb Z)
\cong H_2(A,\mathbb Z)\oplus H_2(B,\mathbb Z)
\oplus\bigl(H_1(A,\mathbb Z)\otimes H_1(B,\mathbb Z)\bigr).
$$

A [cyclic group](../../../../../cyclic-group.md) has zero second integral [group homology](../../../../../group-homology.md), while

$$
C_m\otimes_{\mathbb Z}C_n\cong C_{\gcd(m,n)}.
$$

Consequently

$$
\boxed{M(C_2\times C_4\times C_6)
\cong C_{\gcd(2,4)}\oplus C_{\gcd(2,6)}\oplus C_{\gcd(4,6)}
\cong C_2\oplus C_2\oplus C_2.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 151](../../paper-151-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
