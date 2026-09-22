<h1 id="1/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a definable cumulative hierarchy of set-sized stages: $A_\alpha\subseteq A_\beta$ for $\alpha<\beta$, $A_\eta=\bigcup_{\alpha<\eta}A_\alpha$ at nonzero limits, and $A=\bigcup_{\alpha\in\mathrm{Ord}}A_\alpha$. Class parameters and the hierarchy are fixed definable data. The [reflection theorem for definable hierarchies](../../../../../../../reflection-theorem-for-definable-hierarchies.md) says that for every finite collection $\Phi$ of formulas there is a [closed unbounded class of ordinals](../../../../../../../closed-unbounded-class-of-ordinals.md) $C$ such that

$$
\boxed{\alpha\in C\ \Longrightarrow\
\bigl[A_\alpha\models\varphi(\vec a)\ \Longleftrightarrow\ A\models\varphi(\vec a)\bigr]
\quad(\varphi\in\Phi,\ \vec a\in A_\alpha).}
$$

This is a schema of [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md) for each finite collection and class definition, not a purported truth predicate for all formulas over the universe at once.

Close $\Phi$ under subformulas. For each existential subformula $\exists y\,\psi(y,\vec x)$ and each tuple in $A_\alpha$, if a witness exists in $A$, take the least stage index containing a witness. There are only set-many parameter tuples and finitely many formulas. The [Axiom schema of replacement](../../../../../../../axiom-schema-of-replacement.md) therefore bounds all these least indices by an [ordinal](../../../../../../../ordinal.md) $h(\alpha)$, chosen larger than $\alpha$. No definable selection of the witnesses themselves is needed.

Above any prescribed bound choose $\alpha_0<\alpha_1<\cdots$ with $\alpha_{m+1}>h(\alpha_m)$, and put $\eta=\sup_m\alpha_m$. Every tuple in $A_\eta$ lies in some $A_{\alpha_m}$, and each true existential instance for that tuple has a witness in $A_{\alpha_{m+1}}\subseteq A_\eta$. Induction over the subformulas now proves agreement between $A_\eta$ and $A$: atomic formulas use the same membership relation, Boolean operations preserve agreement, and the existential step uses this witness property. Thus reflecting stages are unbounded.

For closedness, suppose reflecting stages have limit $\eta$. Every tuple in $A_\eta$ lies in a reflecting stage below $\eta$, and every true existential instance has a witness there. The same subformula induction proves reflection at $\eta$. Hence the reflecting stages for the subformula-closed collection form a closed unbounded class, proving the [Lévy reflection theorem](../../../../../../../levy-reflection-theorem.md) in this relative form.

## ↑ Ancestors (12)

1. [A](../a.md)
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
