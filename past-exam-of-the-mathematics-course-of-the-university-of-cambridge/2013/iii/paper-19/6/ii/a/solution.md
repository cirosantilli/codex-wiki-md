<h1 id="6/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a name $\dot f\in M$ for $f$ and a condition $p\in G$ [forcing](../../../../../../../forcing-split.md) that it is a [function](../../../../../../../function-split.md) $\alpha\to\beta$. The [ordinals](../../../../../../../ordinal.md) $\alpha,\beta$ belong to $M$, by [forcing preserves ordinals](../../../../../../../forcing-preserves-ordinals.md). For each $\zeta<\alpha$, choose in $M$ a maximal [forcing antichain](../../../../../../../forcing-antichain.md) $A_\zeta$ in the cone above $p$, every member deciding $\dot f(\zeta)$ as an [ordinal](../../../../../../../ordinal.md) below $\beta$. Conditions deciding an ordinal-valued name are dense, by the [forcing theorem](../../../../../../../forcing-theorem.md).

Let $y(\zeta)$ be the set of values decided by members of $A_\zeta$. The chain condition gives $|y(\zeta)|^M<\kappa$, and Choice and Replacement in $M$ assemble all these sets into a [function](../../../../../../../function-split.md) $y\in M$ with domain $\alpha$. Since $p\in G$, genericity ensures that $G$ meets each deciding [forcing antichain](../../../../../../../forcing-antichain.md) above $p$; equivalently enlarge it to a global maximal [forcing antichain](../../../../../../../forcing-antichain.md) by conditions incompatible with $p$. Its chosen value is the actual $f(\zeta)$. Therefore

$$
\boxed{\operatorname{dom}(y)=\alpha,\quad
M\models|y(\zeta)|<\kappa,\quad
M[G]\models f(\zeta)\in y(\zeta)\text{ for all }\zeta<\alpha.}
$$

This is the [possible-values lemma for chain-condition forcing](../../../../../../../possible-values-lemma-for-chain-condition-forcing.md). All size bounds in its construction are internal to the ground model.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [6](../../../6.md)
4. [Paper 19](../../../../paper-19-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
