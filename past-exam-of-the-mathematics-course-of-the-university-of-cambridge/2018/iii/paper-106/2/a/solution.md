<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual unital-subalgebra convention $I_H\in A$. The [spectral theorem for a commutative operator algebra](../../../../../../spectral-theorem-for-a-commutative-operator-algebra.md) states that the [character space](../../../../../../character-space-of-an-algebra.md) $\Phi_A$, equipped with the [Gelfand topology](../../../../../../gelfand-topology.md), is a [compact Hausdorff space](../../../../../../compact-hausdorff-space.md), and there is a unique regular [projection-valued measure](../../../../../../projection-valued-measure.md) $E$ on its [Borel sigma-algebra](../../../../../../borel-sigma-algebra.md) satisfying

$$
\boxed{E(\Phi_A)=I_H,\qquad a=\int_{\Phi_A}\widehat a(\chi)\,dE(\chi)\quad(a\in A),}
$$

where $\widehat a(\chi)=\chi(a)$ is the [Gelfand transform](../../../../../../gelfand-representation.md). The map $a\mapsto\widehat a$ is an isometric unital star-isomorphism from $A$ onto $C(\Phi_A)$ by the [Commutative Gelfand--Naimark theorem](../../../../../../commutative-gelfand-naimark-theorem.md).

More explicitly, every $E(B)$ is an [orthogonal projection](../../../../../../orthogonal-projection.md), $E(\varnothing)=0$, $E(B\cap C)=E(B)E(C)$, and for disjoint [Borel sets](../../../../../../borel-set.md) $B_n$,

$$
E\left(\bigcup_nB_n\right)v=\sum_nE(B_n)v\quad(v\in H),
$$

with convergence in the norm of the [Hilbert space](../../../../../../hilbert-space-split.md). Regularity means that each [scalar spectral measure](../../../../../../scalar-spectral-measure.md) $B\mapsto\langle E(B)v,w\rangle$ is a [regular Borel measure](../../../../../../regular-borel-measure.md). The integral identity then implies $\|a\|=\sup_{\chi\in\Phi_A}|\widehat a(\chi)|$. No separability assumption on $H$ is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
