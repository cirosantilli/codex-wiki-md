<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work in the ambient universe and let $a,u\in L$. Suppose

$$
L\models\forall x\in a\;\exists!y\;\varphi(x,y,u).
$$

For each $x\in a$, let $y_x$ be this unique witness. The relativization $\varphi^L$ is a first-order formula, so the ambient [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md) collects the witnesses $y_x$ into a set. Every witness lies in the [constructible hierarchy](../../../../../../constructible-hierarchy.md), hence there is an ordinal $\alpha$ such that

$$
\{y_x:x\in a\}\subseteq L_\alpha.
$$

For example, take the supremum of one constructible rank for each witness and then increase it by one.

The set $L_\alpha$ itself belongs to $L_{\alpha+1}\subseteq L$. Taking $b=L_\alpha$, every $x\in a$ has a witness $y\in b$ satisfying $\varphi^L(x,y,u)$. Therefore

$$
L\models\exists b\;\forall x\in a\;\exists y\in b\;\varphi(x,y,u),
$$

which is the stated instance of Replacement.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 128](../../../paper-128-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
