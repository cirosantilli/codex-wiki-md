<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The identity $X_i=\Omega_i-\Omega_{i-1}$ from part (a) shows that each [Young–Jucys–Murphy element](../../../../../../../jucys-murphy-element.md) belongs to the [Gelfand–Tsetlin algebra](../../../../../../../gelfand-tsetlin-algebra.md). Conversely, $Z_r$ lies in the centralizer of $\mathbb C S_{r-1}$ in $\mathbb C S_r$. Applying the preceding [Olshanskii centralizer lemma](../../../../../../../olshanskii-centralizer-lemma.md) at level $r$ gives

$$
Z_r\subseteq\operatorname{alg}(Z_{r-1},X_r).
$$

Induction, beginning with $Z_1=\mathbb C1$, proves $Z_r\subseteq\operatorname{alg}(X_1,\ldots,X_r)$. Thus

$$
\boxed{GZ_n=\operatorname{alg}(X_1,\ldots,X_n)}.
$$

Here every generated algebra is unital; $X_1=0$ causes no problem.

To deduce simple branching, use [Maschke's theorem](../../../../../../../maschke-s-theorem.md): complex representations of finite groups are [semisimple modules](../../../../../../../semisimple-module.md). The [Artin–Wedderburn theorem](../../../../../../../artin-wedderburn-theorem.md) identifies

$$
\mathbb C S_r\cong\bigoplus_L\operatorname{End}_{\mathbb C}(L),
$$

where $L$ runs over the irreducible $S_r$-modules. Write their restrictions as

$$
\operatorname{Res}_{S_{r-1}}^{S_r}L
\cong\bigoplus_M M\otimes\mathbb C^{m_{L,M}}.
$$

By [Schur lemma](../../../../../../../schur-s-lemma.md), the centralizer in the displayed algebra is

$$
Z_{(r-1,1)}\cong
\bigoplus_{L,M}\operatorname{End}_{\mathbb C}(\mathbb C^{m_{L,M}}),
$$

with zero multiplicities omitted. Part (i) makes this algebra commutative, whereas a full [matrix algebra](../../../../../../../matrix-algebra.md) of size at least two is noncommutative. Consequently **every restriction multiplicity is $0$ or $1$**. This proves [multiplicity-free restriction](../../../../../../../multiplicity-free-restriction.md) at each step, with no use of the branching rule in the centralizer proof.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
