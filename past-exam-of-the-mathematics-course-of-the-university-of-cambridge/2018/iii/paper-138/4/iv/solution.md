<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Completeness permits [idempotent lifting](../../../../../../idempotent-lifting.md) from $kG$ to $\mathcal OG$. In particular, each [projective cover](../../../../../../projective-cover.md) $P_j$ lifts to a finite projective $\mathcal OG$-lattice $\widetilde P_j$; one can lift an idempotent presenting it as a summand of a [finite free module](../../../../../../finite-free-module.md). Set $Q_j=K\otimes_{\mathcal O}\widetilde P_j$.

For a simple $S_\ell$, every map $P_j\to S_\ell$ factors through its simple head $S_j$. Splitting and [Schur lemma](../../../../../../schur-s-lemma.md) give $\dim_k\operatorname{Hom}_{kG}(P_j,S_\ell)=\delta_{j\ell}$. Exactness of this Hom functor along a [composition series](../../../../../../composition-series.md) therefore gives

$$
\dim_k\operatorname{Hom}_{kG}(P_j,\overline W_i)=d_{ij}.
$$

Part (iii) identifies this with $\dim_K\operatorname{Hom}_{KG}(Q_j,V_i)$. By [Maschke's theorem](../../../../../../maschke-s-theorem.md) and splitting, $KG$ is split semisimple, so

$$
Q_j\cong\bigoplus_i V_i^{\oplus d_{ij}}.
$$

The reductions of any two integral forms of the same ordinary module have identical [Brauer characters](../../../../../../brauer-character.md), hence identical composition multiplicities. We may thus reduce a direct-sum form for the displayed decomposition instead of $\widetilde P_j$. In the [modular representation ring](../../../../../../modular-representation-ring.md) this gives

$$
[P_j]=\sum_i d_{ij}[\overline W_i]=\sum_\ell\left(\sum_i d_{i\ell}d_{ij}\right)[S_\ell].
$$

Comparing the simple basis coefficients proves $c_{\ell j}=\sum_i d_{i\ell}d_{ij}$, or $\boxed{C=D^TD}$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
