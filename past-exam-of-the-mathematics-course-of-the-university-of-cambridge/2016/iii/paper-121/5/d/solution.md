<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Closure preserves the ground-model cardinal $\lambda$.** We use the stronger fact that [closed forcing adds no short ordinal sequences](../../../../../../closed-forcing-adds-no-short-ordinal-sequences.md). Fix an ordinal $\mu<\lambda$ in $M$ and a [forcing name](../../../../../../forcing-name.md) $\dot h$ that a condition $p$ forces to be an ordinal-valued function with domain $\mu$.

Inside $M$, recursively strengthen $p$ to decide each value $\dot h(\xi)$, for $\xi<\mu$. At a limit stage take a lower bound of the previously chosen descending sequence; its length is below $\lambda$, so $\lambda$-closure supplies one. After all $\mu$ values have been decided, closure supplies a common lower bound $q$. The decided values form a function $h\in M$ by the [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md), and

$$
q\Vdash\dot h=\check h.
$$

The recursion is carried out within $M$ using the definable [forcing theorem](../../../../../../forcing-theorem.md) and a ground-model choice of deciding extensions, so every sequence to which closure is applied belongs to $M$. Repeating the construction below any stronger condition shows that such full-decision conditions are [dense below a forcing condition](../../../../../../dense-below-a-forcing-condition.md) $p$. The [dense-below generic meeting lemma](../../../../../../dense-below-generic-meeting-lemma.md) ensures that a [generic filter](../../../../../../generic-filter.md) containing $p$ meets them. Thus the interpreted function is in $M$.

If $\lambda$ ceased to be a [cardinal number](../../../../../../cardinal-number.md) in $M[G]$, there would be a surjection $\mu\to\lambda$ for some ordinal $\mu<\lambda$. The [forcing theorem](../../../../../../forcing-theorem.md) gives a name and a condition in $G$ forcing this. The argument above makes its interpretation a ground-model function, but $M$ regards $\lambda$ as a [cardinal number](../../../../../../cardinal-number.md) and admits no such surjection. Therefore

$$
\boxed{M[G]\models\text{“}\lambda\text{ is a cardinal”}}.
$$

No regularity of $\lambda$ is required; every recursion used has length strictly below $\lambda$. Finite cardinals are preserved automatically. This is [cardinal preservation by closed forcing](../../../../../../cardinal-preservation-by-closed-forcing.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
