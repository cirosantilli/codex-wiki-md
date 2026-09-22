<h1 id="1/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The printed inclusion-and-elementarity assertion is false if transitivity is required of the same submodel.** Take the theorem of [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md) that combines the [axiom of infinity](../../../../../../../axiom-of-infinity.md) and the [Axiom of power set](../../../../../../../axiom-of-power-set.md). Whenever $V_\delta$ satisfies this sentence, it contains $\omega$, every [subset](../../../../../../../subset.md) of $\omega$, and their actual [power set](../../../../../../../power-set.md) $\mathcal P(\omega)$. A submodel $M\prec V_\delta$ contains $\omega$ and $\mathcal P(\omega)$, since these are uniquely definable in $V_\delta$. If $M$ were transitive, it would contain every element of $\mathcal P(\omega)$, contradicting countability by [Cantor theorem](../../../../../../../cantor-s-theorem.md).

The corrected conclusion uses an [elementary embedding](../../../../../../../elementary-embedding.md) rather than elementary inclusion. By [Lévy reflection theorem](../../../../../../../levy-reflection-theorem.md), choose $\delta>\omega+2$ with $V_\delta\models\varphi$ and with Extensionality true there. The [Downward Lowenheim-Skolem theorem](../../../../../../../downward-lowenheim-skolem-theorem.md) says that an infinite structure in a countable language has a countable [elementary substructure](../../../../../../../elementary-substructure.md). Apply it to obtain a countable $N\prec(V_\delta,\in)$. The membership relation on $N$ is externally well-founded, and elementarity makes it extensional. The [Mostowski collapse theorem](../../../../../../../mostowski-collapse-theorem.md) gives an isomorphism $\pi:N\to M$ onto a countable [transitive set](../../../../../../../transitive-set.md). Hence

$$
\boxed{M\models\varphi,\qquad j=\pi^{-1}:M\longrightarrow V_\delta
\text{ is elementary}.}
$$

Indeed $M\subseteq V_\delta$: rank induction gives $\operatorname{rank}(\pi(x))\le\operatorname{rank}(x)$ for every $x\in N$. The crucial correction is that **$j$, rather than the inclusion of $M$, is elementary**. For a formula with free variables, apply this argument to its universal closure.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [1](../../../1.md)
4. [Paper 19](../../../../paper-19-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
