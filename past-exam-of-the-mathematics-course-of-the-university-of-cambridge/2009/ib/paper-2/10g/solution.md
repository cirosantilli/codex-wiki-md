<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

The ascending chain $\ker T\subseteq\ker T^2\subseteq\cdots$ must stabilize because $V$ is finite-dimensional. Once $\ker T^l=\ker T^{l+1}$, it stays stable: if $T^{l+2}v=0$, then $Tv\in\ker T^{l+1}=\ker T^l$, so $v\in\ker T^{l+1}=\ker T^l$; induction repeats the argument. Choose a positive such $l$, giving $\ker T^{2l}=\ker T^l$.

If $v\in\ker T^l\cap\operatorname{im}T^l$, write $v=T^lw$. Then $T^{2l}w=0$, so $w\in\ker T^l$ and $v=0$. By the [rank-nullity theorem](../../../../../rank-nullity-theorem.md), the dimensions of those two subspaces sum to $\dim V$. Hence

$$
\boxed{V=\ker T^l\oplus\operatorname{im}T^l.}
$$

This proves the finite-dimensional form of the [Fitting lemma](../../../../../fitting-lemma.md).

If $\det T=0$, the [kernel](../../../../../kernel-of-a-linear-map.md) contains a nonzero [vector](../../../../../vector.md) $u$, and $\operatorname{im}T$ is a proper [vector subspace](../../../../../vector-subspace.md). Extend a [basis](../../../../../basis.md) of that [image of a linear map](../../../../../image-of-a-linear-map.md) to a [basis](../../../../../basis.md) of $V$ and choose a nonzero [linear functional](../../../../../linear-functional.md) $\lambda$ which vanishes on the former [basis](../../../../../basis.md). Define $S(v)=\lambda(v)u$. It is a nonzero [endomorphism](../../../../../endomorphism.md), since $\lambda$ takes a nonzero value somewhere, and

$$
TS(v)=\lambda(v)Tu=0,\qquad ST(v)=\lambda(Tv)u=0.
$$

Thus **a [singular endomorphism has a nonzero two-sided annihilator](../../../../../singular-endomorphism-has-a-nonzero-two-sided-annihilator.md)**, as required.

For an [idempotent linear map](../../../../../projection-linear-algebra.md) $T$, the decomposition $v=(v-Tv)+Tv$ shows $V=\ker T\oplus\operatorname{im}T$: the first term is killed by $T$, the second is fixed, and a [vector](../../../../../vector.md) both fixed and killed is zero. An adapted [basis](../../../../../basis.md) makes its [matrix](../../../../../matrix.md) $\operatorname{diag}(0,I_r)$, with $r=\operatorname{rank}T$. Consequently equal ranks give identical adapted [matrices](../../../../../matrix.md) and therefore a change of [basis](../../../../../basis.md) relating $T_1,T_2$. Conversely, similar [matrices](../../../../../matrix.md) have the same rank because pre- and postmultiplication by [invertible matrices](../../../../../invertible-matrix.md) preserve rank. Hence **$T_1$ and $T_2$ are similar exactly when their ranks agree**, proving the [similarity classification of idempotent linear maps](../../../../../similarity-classification-of-idempotent-linear-maps.md).

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
