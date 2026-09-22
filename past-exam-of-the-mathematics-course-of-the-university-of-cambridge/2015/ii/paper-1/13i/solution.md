<h1 id="13i/solution">Solution</h1>

↑ **Parent:** [13I](../13i.md)

The [completeness theorem for propositional logic](../../../../../completeness-theorem-for-propositional-logic.md) states that $S\models\phi$ if and only if $S\vdash\phi$. Soundness follows by checking that axioms are tautologies and inference rules preserve truth. For completeness it suffices to prove that every syntactically consistent set has a model.

The [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md) used here is: $S\cup\{\psi\}\vdash\chi$ if and only if $S\vdash\psi\Rightarrow\chi$, in classical propositional logic. A proof is finite, so the union of a chain of consistent sets remains consistent: a contradiction would already occur in one member. By [Zorn's lemma](../../../../../zorn-s-lemma.md), extend a consistent $S$ to a maximal consistent set $T$. If $\psi\notin T$, adding $\psi$ yields a contradiction; the deduction theorem gives $T\vdash\neg\psi$, and maximal consistency puts $\neg\psi$ in $T$. Conversely $\psi$ and $\neg\psi$ cannot both belong to $T$. Maximal consistency also makes $T$ deductively closed.

Assign each primitive proposition the truth value true precisely when it belongs to $T$. The [maximal consistent set truth lemma](../../../../../maximal-consistent-set-truth-lemma.md) follows by induction on formulas. For negation use the preceding dichotomy. For implication, if $\neg\psi\in T$ or $\chi\in T$, the classical implication axioms put $\psi\Rightarrow\chi$ in $T$; if $\psi\in T$ and $\neg\chi\in T$, modus ponens prevents that implication from belonging to $T$. This is exactly its truth table. Other connectives are defined from these or handled by the same induction. The resulting valuation satisfies all of $T$, hence all of $S$.

If $S\nvdash\phi$, the deduction theorem and classical contradiction rules show $S\cup\{\neg\phi\}$ is consistent. Its model falsifies $\phi$, so $S\not\models\phi$. This proves **completeness**.

The [propositional compactness theorem](../../../../../propositional-compactness-theorem.md) says $S$ is satisfiable if every finite subset is satisfiable. Otherwise completeness would make $S$ inconsistent, and a finite proof of contradiction would involve only finitely many assumptions, contradicting their satisfiability. Equivalently, every semantic consequence of $S$ is a consequence of a finite subset. The [decidability theorem for propositional logic](../../../../../decidability-theorem-for-propositional-logic.md) says there is an algorithm deciding whether a formula is provable with no assumptions: enumerate all truth assignments to its finitely many primitive propositions, check whether it is a tautology, and use soundness and completeness to identify tautologies with theorems. This does not claim an algorithm for arbitrary infinitely presented theories.

Finally, the valuation assigning false to every $p_n$ satisfies all the implications in $S$ and falsifies $p_1$. By soundness, **$S\nvdash p_1$**.

## ↑ Ancestors (10)

1. [13I](../13i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
