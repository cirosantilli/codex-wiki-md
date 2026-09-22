<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

The [completeness theorem for propositional logic](../../../../../completeness-theorem-for-propositional-logic.md) states that $\Gamma\models\phi$ implies $\Gamma\vdash\phi$: every semantic consequence is formally derivable. Equivalently, every syntactically consistent set of formulas has a truth assignment satisfying it.

First prove the equivalent formulation. With countably many primitive propositions there are countably many formulas; enumerate them as $\phi_1,\phi_2,\ldots$. Starting from a consistent $\Gamma$, construct increasing consistent sets $\Gamma_n$ by adjoining $\phi_n$ if this remains consistent, and otherwise adjoining $\neg\phi_n$. The second choice is consistent: if adjoining either choice were inconsistent, the [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md) would give both $\neg\phi_n$ and $\neg\neg\phi_n$ as consequences of $\Gamma_{n-1}$, contradicting consistency.

The union $\Delta=\bigcup_n\Gamma_n$ is consistent, since a finite proof of a contradiction would already use premises in one stage. It decides every formula. It is also deductively closed: if $\Delta\vdash\psi$ and $\psi\notin\Delta$, then $\neg\psi\in\Delta$, violating consistency.

Give an atomic proposition $P$ the truth value true exactly when $P\in\Delta$. Induction proves the truth lemma. For negation, exactly one of $\psi,\neg\psi$ lies in $\Delta$. For implication, if $\psi\to\chi\in\Delta$ and $\psi\in\Delta$, modus ponens gives $\chi\in\Delta$. Conversely, if $\psi\notin\Delta$, then $\neg\psi\in\Delta$ entails $\psi\to\chi$ by a classical propositional tautology; if $\chi\in\Delta$, it too entails $\psi\to\chi$. Hence membership of an implication agrees with its truth table. Other connectives follow from their definitions or the corresponding tautologies. Thus the assignment satisfies $\Delta$, and therefore $\Gamma$.

Now if $\Gamma\nvdash\phi$, the set $\Gamma\cup\{\neg\phi\}$ is consistent, by the [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md) and classical double-negation elimination. Its satisfying assignment is a model of $\Gamma$ in which $\phi$ is false. Contraposition proves

$$
\boxed{\Gamma\models\phi\ \Longrightarrow\ \Gamma\vdash\phi.}
$$

The reverse implication is [soundness theorem for propositional logic](../../../../../soundness-theorem-for-propositional-logic.md), proved by checking axioms and inference rules preserve truth.

For uncountably many primitive propositions, replace the enumeration by a maximal-consistent extension using [Zorn lemma](../../../../../zorn-s-lemma.md). The union of a chain of consistent extensions is consistent for the same finite-proof reason. Maximality then decides each formula: if adjoining $\psi$ creates inconsistency, the deduction argument gives $\neg\psi$ already in the extension. The same truth lemma applies with no change. Alternatively, well-order the formulas and run the same recursion with unions at limit stages. This modification uses a choice principle, unlike the countable enumeration argument.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
