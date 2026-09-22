<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the logical truth constants $\top,\bot$, and put

$$
A'=A[p:=\top],\qquad A''=A[p:=\bot].
$$

For a truth assignment with $p$ true, $A$ has the value of $A'$ and $(A'\wedge p)\vee(A''\wedge\neg p)$ has the same value. For an assignment with $p$ false, both have the value of $A''$. Thus the [propositional variable elimination](../../../../../../propositional-variable-elimination.md) identity is

$$
\boxed{A\equiv(A[p:=\top]\wedge p)\vee(A[p:=\bot]\wedge\neg p).}
$$

Neither substituted formula contains $p$.

Let $P=\operatorname{Var}(A)\setminus\operatorname{Var}(B)$, and eliminate all the private letters of $A$ by taking

$$
C=\bigvee_{\varepsilon:P\to\{0,1\}}A[P:=\varepsilon],
$$

where a Boolean assignment substitutes $\top$ or $\bot$ for each letter. Then $\operatorname{Var}(C)\subseteq\operatorname{Var}(A)\cap\operatorname{Var}(B)$. Every assignment satisfying $A$ satisfies the disjunct corresponding to its own private-letter values, so $A\models C$.

If an assignment satisfies $C$, choose a disjunct witnessing this, and modify only its values on $P$ to the corresponding $\varepsilon$. The modified assignment satisfies $A$, hence satisfies $B$ by soundness of $A\vdash B$. Its values on every letter of $B$ have remained unchanged, so the original assignment also satisfies $B$. Therefore $C\models B$. The [propositional completeness theorem](../../../../../../completeness-theorem-for-propositional-logic.md) converts these two valid implications into

$$
\boxed{A\vdash C\quad\text{and}\quad C\vdash B,}
$$

proving [propositional interpolation](../../../../../../propositional-interpolation.md) constructively.

If the syntax does not initially include $\top,\bot$, they can be admitted as logical constants without adding propositional letters. This convention matters when the common vocabulary is empty: a grammar in which every formula must contain a letter has no letter-free interpolant at all. For example, two tautologies using disjoint letters entail one another but cannot have an interpolant in that grammar. The truth-constant convention supplies exactly the necessary empty-vocabulary case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
