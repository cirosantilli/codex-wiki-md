<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The preceding parts give a simple [Specht module](../../../../../../specht-module.md) for each partition and show that different partitions give nonisomorphic simples. The [conjugacy classes](../../../../../../conjugacy-class.md) of $S_n$ are indexed by partitions of $n$, namely cycle types. We use the standard finite-group character theorem: the number of irreducible complex characters equals the number of [conjugacy classes](../../../../../../conjugacy-class.md), and they form an orthonormal basis of complex [class functions](../../../../../../class-function.md). Consequently the $\chi^\lambda$ are the complete list of [irreducible characters](../../../../../../irreducible-character.md) of $S_n$.

By [Maschke's theorem](../../../../../../maschke-s-theorem.md), the [Young permutation module](../../../../../../young-permutation-module.md) $M^\mu$ decomposes as a [direct sum](../../../../../../direct-sum.md) of these simple modules. For a semisimple complex module, [Schur lemma](../../../../../../schur-s-lemma.md) makes the multiplicity of a simple module equal to the dimension of the homomorphism space from that simple; [character orthogonality](../../../../../../character-orthogonality.md) identifies the same number with the [character inner product](../../../../../../character-inner-product.md). Hence

$$
M^\mu\cong\bigoplus_{\lambda\vdash n}(S^\lambda)^{\oplus a_{\lambda\mu}},\qquad a_{\lambda\mu}=\dim\operatorname{Hom}_{\mathbb CS_n}(S^\lambda,M^\mu)=\langle\xi^\mu,\chi^\lambda\rangle\in\mathbb Z_{\geq0}.
$$

Part (ii) makes $a_{\lambda\mu}=0$ unless $\lambda\unrhd\mu$, and gives $a_{\mu\mu}=1$. Taking characters proves

$$
\boxed{\xi^\mu=\sum_{\lambda\unrhd\mu}\langle\xi^\mu,\chi^\lambda\rangle\chi^\lambda,\qquad\langle\xi^\mu,\chi^\mu\rangle=1.}
$$

Thus the permutation-character decomposition is triangular in the [dominance order on partitions](../../../../../../dominance-order-on-partitions.md), with diagonal multiplicity one. These are the dominance and diagonal-multiplicity consequences of [Young's rule](../../../../../../young-s-rule.md), obtained here without assuming its full multiplicity formula.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
