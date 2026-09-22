<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [definable continuous hierarchy](../../../../../../definable-continuous-hierarchy.md) is a definable class function $\alpha\mapsto H_\alpha$ on the [ordinals](../../../../../../ordinal.md), with set-valued levels, such that $H_\alpha\subseteq H_\beta$ for $\alpha<\beta$ and

$$
H_\lambda=\bigcup_{\alpha<\lambda}H_\alpha
$$

for nonzero [limit ordinals](../../../../../../limit-ordinal.md). Its union is a definable [class in set theory](../../../../../../class-set-theory.md) $H$. Often the definition additionally requires every level to be a [transitive set](../../../../../../transitive-set.md); the following statement also works without that requirement.

The [reflection theorem for definable hierarchies](../../../../../../reflection-theorem-for-definable-hierarchies.md) says that for any finite collection $\mathcal F$ of [first-order formulas](../../../../../../first-order-formula.md), there is a [closed unbounded](../../../../../../club-set.md) class of [ordinals](../../../../../../ordinal.md) $\alpha$ such that, for every $\varphi\in\mathcal F$ and every parameter tuple from $H_\alpha$,

$$
\boxed{(H_\alpha,\in)\models\varphi(\vec a)\ \Longleftrightarrow\ (H,\in)\models\varphi(\vec a).}
$$

A useful justification is the witness-closure proof. Close $\mathcal F$ under subformulas. At each level and for each existential subformula, bound the least level containing a witness for each parameter tuple for which a witness exists in $H$. [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md) bounds these indices. Iterating the finitely many bounds through $\omega$ produces a limit level containing all required witnesses. Induction on the [first-order formulas](../../../../../../first-order-formula.md), equivalently the finite-formula version of the [Tarski-Vaught test](../../../../../../tarski-vaught-test.md), yields agreement. Continuity gives closedness of the reflecting class, and starting above any prescribed [ordinal](../../../../../../ordinal.md) gives unboundedness. This is finite reflection, not a claim that all [first-order formulas](../../../../../../first-order-formula.md) reflect simultaneously in an arbitrary hierarchy.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
