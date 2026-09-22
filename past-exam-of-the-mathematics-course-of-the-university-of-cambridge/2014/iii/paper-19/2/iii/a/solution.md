<h1 id="2/iii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $a,\vec p\in L$ and a formula $\theta(x,\vec p)$. The [reflection theorem for definable hierarchies](../../../../../../../reflection-theorem-for-definable-hierarchies.md) supplies a stage $L_\beta$ containing these parameters at which the finitely many subformulas of $\theta$ have the same truth values as in $L$, for arguments in $L_\beta$.

This reflection can be proved in the ambient [ZF](../../../../../../../zermelo-fraenkel-set-theory.md) without presupposing [Axiom schema of separation](../../../../../../../axiom-schema-of-specification.md) in $L$: starting at a stage containing the parameters, collect for each relevant existential subformula and every tuple in the current stage the least constructible stage in which a witness occurs, whenever a witness exists in $L$. Ambient [Axiom schema of replacement](../../../../../../../axiom-schema-of-replacement.md) bounds these [ordinals](../../../../../../../ordinal.md). Iterate these witness-stage bounds for $\omega$ steps and take their supremum. Induction on subformulas gives the required finite reflection at the resulting union stage. Only the least stage is chosen, so no ambient [axiom of choice](../../../../../../../axiom-of-choice.md) is needed.

Since $L_\beta$ is transitive and contains $a$, the desired separated [subset](../../../../../../../subset.md) is

$$
b=\{x\in L_\beta:x\in a\text{ and }(L_\beta,\in)\models\theta(x,\vec p)\}.
$$

It is definable over $L_\beta$ with parameters there, so $b\in\operatorname{Def}(L_\beta)=L_{\beta+1}\subset L$. Reflection gives $b=\{x\in a:\theta^L(x,\vec p)\}$. Hence **[ZF](../../../../../../../zermelo-fraenkel-set-theory.md) proves every [Axiom schema of separation](../../../../../../../axiom-schema-of-specification.md) instance relativized to $L$**. This is a direct [Separation proof in the constructible universe](../../../../../../../separation-proof-in-the-constructible-universe.md), not an appeal to the assertion being proved.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Iii](../../iii.md)
3. [2](../../../2.md)
4. [Paper 19](../../../../paper-19-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
