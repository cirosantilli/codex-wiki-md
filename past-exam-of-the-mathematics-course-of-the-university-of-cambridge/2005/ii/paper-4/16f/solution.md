<h1 id="16f/solution">Solution</h1>

↑ **Parent:** [16F](../16f.md)

The [propositional completeness theorem](../../../../../completeness-theorem-for-propositional-logic.md) states that $\Gamma\models\phi$ if and only if $\Gamma\vdash\phi$. Soundness follows by checking the axioms against truth [valuations](../../../../../valuation.md) and noting that [modus ponens rule](../../../../../implication-elimination-rule.md) preserves truth. For completeness, use the [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md): if $\Gamma\cup\{p\}\vdash q$, then $\Gamma\vdash p\Rightarrow q$. In the usual negation rules this also says that a contradiction from $\Gamma\cup\{p\}$ proves $\Gamma\vdash\neg p$.

First construct a maximal consistent set extending any consistent set $\Delta$. Enumerate all formulas, possible because the primitive propositions are countable. Starting with $\Delta_0=\Delta$, add formula $\psi_n$ at step $n$ if consistency is preserved; otherwise add $\neg\psi_n$. This latter addition is consistent: if both extensions gave contradictions, the [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md) would prove both $\neg\psi_n$ and $\neg\neg\psi_n$ from $\Delta_n$, a contradiction already in $\Delta_n$. The union $M$ is consistent because a finite proof uses only finitely many newly added premises. It decides every formula: exactly one of $\psi,\neg\psi$ belongs to $M$. It is deductively closed, since an omitted derivable formula would have its negation in $M$, contradicting consistency.

Assign a [valuation](../../../../../valuation.md) $v(p)=1$ exactly when the primitive proposition $p$ lies in $M$. Structural induction proves the [maximal consistent set truth lemma](../../../../../maximal-consistent-set-truth-lemma.md) $v(\psi)=1$ if and only if $\psi\in M$. Negation follows from the decision property. For implication, if $\psi\Rightarrow\chi\in M$ and $\psi\in M$, [modus ponens rule](../../../../../implication-elimination-rule.md) gives $\chi\in M$. Conversely, if $\chi\in M$, the elementary implication axioms give $\psi\Rightarrow\chi\in M$. If $\psi\notin M$, then $\neg\psi\in M$, and the usual contradiction rule proves $\psi\Rightarrow\chi$. These two alternatives match the [truth table](../../../../../truth-table.md). The other connectives, if primitive, are handled by their corresponding rules or defined from negation and implication. Thus every consistent set has a [valuation](../../../../../valuation.md) satisfying it.

Now suppose $\Gamma\not\vdash\phi$. If $\Gamma\cup\{\neg\phi\}$ were inconsistent, the [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md) would give $\Gamma\vdash\neg\neg\phi$. **Here the third axiom $\neg\neg\phi\Rightarrow\phi$ is essential:** it would give $\Gamma\vdash\phi$, a contradiction. Hence that extension is consistent and has a satisfying [valuation](../../../../../valuation.md). This [valuation](../../../../../valuation.md) satisfies $\Gamma$ and falsifies $\phi$, proving the contrapositive of completeness. In this organization of the proof, the explicit classical double-negation elimination occurs in this last consistency step; the construction and truth lemma use the ordinary negation and contradiction rules, not an unmentioned identification of $\neg\neg\phi$ with $\phi$.

The [propositional compactness theorem](../../../../../propositional-compactness-theorem.md) says that a set of formulas is satisfiable exactly when each finite subset is satisfiable. If it were not satisfiable, completeness would make it inconsistent. Its finite contradiction proof uses only a finite subset of premises; soundness makes that subset unsatisfiable. This contradicts the assumed finite satisfiability and proves compactness.

## ↑ Ancestors (10)

1. [16F](../16f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
