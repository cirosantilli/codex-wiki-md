<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Godel completeness theorem](../../../../../../godel-s-completeness-theorem.md) is strong completeness: for any [first-order theory](../../../../../../first-order-theory.md) $T$ and sentence $\sigma$,

$$
\boxed{T\models\sigma\quad\Longleftrightarrow\quad T\vdash\sigma.}
$$

Equivalently every syntactically consistent theory has a model. Work in the ordinary classical metatheory with choice; the language need not be countable. Soundness is induction on a derivation: logical axioms hold under every assignment, modus ponens preserves truth, and the quantifier rule preserves truth when its variable is not free in the assumptions. We prove the nontrivial converse by a [Henkin construction](../../../../../../henkin-construction.md).

Start with a consistent $T$ and add a constant if the language has no closed term. Let $L_0$ be this language. At stage $n$, for every existential sentence $\exists x\,\varphi(x)$ of $L_n$, add a fresh constant $c_\varphi$ and the witness axiom

$$
\exists x\,\varphi(x)\longrightarrow\varphi(c_\varphi).
$$

An axiom of this form is conservative for consistency: if a contradiction followed after adding it, the old theory would prove its negation, hence both $\exists x\,\varphi(x)$ and $\neg\varphi(c_\varphi)$. Since the constant is fresh, replace it by a fresh variable and generalize, obtaining $\forall x\,\neg\varphi(x)$, a contradiction. Every finite [set](../../../../../../set-split.md) of new witness axioms can be handled one at a time, so each stage remains consistent. Their union $T_H$ is consistent because a finite proof uses only finitely many stages.

Well-order the sentences of $L_H=\bigcup_nL_n$. Successively add a sentence if doing so is consistent, and otherwise add its negation. At least one of those two choices preserves consistency: otherwise the deduction theorem would give both its negation and its double negation in the previous theory. At limits take unions. The deductive closure $\Gamma$ of the resulting union is complete and consistent and retains all witness axioms. Every sentence of $L_H$ uses finitely many symbols and belongs to some $L_n$, so its existential witness was added at the next stage. Thus $\Gamma$ has the [Henkin witness property](../../../../../../henkin-witness-property.md) even for formulas using the new constants.

Build its [term model](../../../../../../term-model.md). The domain consists of closed terms modulo $s\sim t$ iff $\Gamma\vdash s=t$. Equality axioms make this an equivalence relation and a congruence. Interpret functions by forming their corresponding terms, and interpret a relation $R$ by $R([t_1],\ldots,[t_r])$ iff $R(t_1,\ldots,t_r)\in\Gamma$. Congruence makes this independent of representatives.

The [truth lemma for a Henkin term model](../../../../../../truth-lemma-for-a-henkin-term-model.md) is proved by induction on formulas after substituting closed terms for their free variables. Atomic formulas are the definition. Completeness and consistency of $\Gamma$ give the Boolean steps. For existence, if $\exists x\,\varphi(x,\bar t)\in\Gamma$, a witness axiom yields a constant $c$ with $\varphi(c,\bar t)\in\Gamma$, and induction supplies a model witness. Conversely every domain element is a term class, so a model witness gives an instance in $\Gamma$, and existential introduction gives the existential sentence. Universality follows by negation and existence. The model therefore satisfies $\Gamma$, hence $T$.

Finally, if $T\nvdash\sigma$, then $T\cup\{\neg\sigma\}$ is consistent by the deduction theorem and classical logic. Its constructed model is a countermodel to $T\models\sigma$. This proves completeness, with an actual witness model rather than merely a finite-satisfiability assertion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
