<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Replace each implication by a [logical disjunction](../../../../../logical-disjunction.md) and use the [conjunctive normal form](../../../../../conjunctive-normal-form.md) for [exclusive or](../../../../../exclusive-or.md) from part (a). The resulting [Boolean clauses](../../../../../clause-of-a-boolean-formula.md) are

$$
\begin{array}{c|l}
F_1&C_1=\neg H\lor Y\\
F_2&C_2=\neg T\lor\neg I\\
F_3&C_3=H\lor T,\quad C_4=\neg H\lor\neg T\\
F_4&C_5=Y\lor I,\quad C_6=\neg Y\lor\neg I.
\end{array}
$$

Here the displayed array is a list of the six [Boolean clauses](../../../../../clause-of-a-boolean-formula.md), whose [logical conjunction](../../../../../logical-conjunction.md) is equivalent to all four constraints.

Use [resolution](../../../../../resolution.md) first on $I$, then on $T$, and finally on $H$:

$$
\begin{aligned}
C_7&=\operatorname{Res}_{I}(C_2,C_5)=\neg T\lor Y,\\
C_8&=\operatorname{Res}_{T}(C_3,C_7)=H\lor Y,\\
C_9&=\operatorname{Res}_{H}(C_1,C_8)=Y\lor Y=\boxed{Y.}
\end{aligned}
$$

Removing the repeated [Boolean literal](../../../../../boolean-literal.md) in the final [Boolean clause](../../../../../clause-of-a-boolean-formula.md) uses idempotence. Neither $C_4$ nor $C_6$ is needed: even the weaker assumptions that the coin has at least one outcome and that at least one person wins already force $Y$, once the two implications hold.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
