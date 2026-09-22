<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A proper [filter on a set](../../../../../filter-set-theory.md) $I$ contains $I$, excludes $\varnothing$, is upward closed, and is closed under finite intersections. Order its proper extensions by inclusion. The union of a nonempty chain is again a proper filter: finitely many members lie together in one chain member. [Zorn lemma](../../../../../zorn-s-lemma.md), and hence the [axiom of choice](../../../../../axiom-of-choice.md), gives a maximal extension $\mathcal U$. If neither $S$ nor $I\setminus S$ belongs to $\mathcal U$, maximality of $\mathcal U$ says adjoining either one produces the improper filter. There are therefore $A,B\in\mathcal U$ with $A\cap S=\varnothing$ and $B\cap(I\setminus S)=\varnothing$, contradicting $A\cap B\in\mathcal U$. Thus $\mathcal U$ is an [ultrafilter](../../../../../ultrafilter.md).

For [Łoś theorem](../../../../../los-theorem.md), interpret the [ultraproduct](../../../../../ultraproduct.md) using $a\sim b$ when $\{i:a_i=b_i\}\in\mathcal U$, with functions and relations interpreted coordinatewise. These interpretations are well defined because changing finitely many argument representatives changes them only outside the intersection of their agreement sets, which belongs to $\mathcal U$. For any [first-order formula](../../../../../first-order-formula.md) and sequences of parameters,

$$
\boxed{\prod_i\mathfrak M_i/\mathcal U\models\phi([\mathbf a])\quad\Longleftrightarrow\quad S_\phi(\mathbf a):=\{i:\mathfrak M_i\models\phi(\mathbf a_i)\}\in\mathcal U.}
$$

Prove this by [structural induction](../../../../../structural-induction.md). Atomic formulas follow from the interpretation of terms. Conjunction uses finite intersections; negation uses the [ultrafilter](../../../../../ultrafilter.md) dichotomy between a set and its complement. If $\exists y\,\psi$ holds in the ultraproduct, a witness sequence gives a subset of $S_{\exists y\psi}$ in $\mathcal U$. Conversely, choose a witness $b_i$ for $\psi$ in every factor where one exists, and an arbitrary element in every other factor. This is the second explicit use of the [axiom of choice](../../../../../axiom-of-choice.md); all factors have nonempty carriers. The inductive hypothesis applied to $\psi(\mathbf a,\mathbf b)$ supplies the ultraproduct witness. The other connectives and universal quantification follow from these cases.

For the possible worlds, use [free filters](../../../../../free-filter.md), equivalently proper filters extending the [cofinite filter](../../../../../cofinite-filter.md) $F_0$. Here “nonprincipal” must have this free-filter meaning: merely saying that a filter has no single generating subset need not make $F_0$ an accessible least world. The designated world is $F_0$, and all worlds have carrier $D=\prod_iM_i$. Atoms, including equality, are forced by

$$
F\Vdash\phi(\mathbf a)\quad\Longleftrightarrow\quad S_\phi(\mathbf a)\in F.
$$

Equality may identify distinct sequences at a world; it is a persistent congruence, and at an ultrafilter world its quotient is the ordinary ultraproduct.

The required equivalence with all ultraproducts uses [dense-extension filter semantics](../../../../../dense-extension-filter-semantics.md). Its recursive clauses are

$$
\begin{aligned}
F\Vdash\bot&\quad\text{never},\\
F\Vdash\phi\land\psi&\iff F\Vdash\phi\text{ and }F\Vdash\psi,\\
F\Vdash\neg\phi&\iff\forall G\supseteq F\;(G\not\Vdash\phi),\\
F\Vdash\phi\to\psi&\iff\forall G\supseteq F\;(G\Vdash\phi\Rightarrow G\Vdash\psi),\\
F\Vdash\phi\lor\psi&\iff\forall G\supseteq F\;\exists H\supseteq G\;(H\Vdash\phi\text{ or }H\Vdash\psi),\\
F\Vdash\exists x\,\phi(x)&\iff\exists a\in D\;(F\Vdash\phi(a)),\\
F\Vdash\forall x\,\phi(x)&\iff\forall G\supseteq F\;\forall a\in D\;(G\Vdash\phi(a)).
\end{aligned}
$$

Every extension in these clauses is a free proper filter. The dense clause for disjunction is essential; for propositional formulas, local disjunction would instead give a [Kripke model for intuitionistic propositional logic](../../../../../kripke-model-for-intuitionistic-propositional-logic.md) and would invalidate the claimed equivalence.

The useful separation fact is [membership in a free filter is detected by its ultrafilter extensions](../../../../../membership-in-a-free-filter-is-detected-by-its-ultrafilter-extensions.md):

$$
S\in F\iff\forall\mathcal U\supseteq F\;(\mathcal U\text{ a nonprincipal ultrafilter}\Rightarrow S\in\mathcal U).
$$

Indeed, if $S\notin F$, every $A\in F$ has infinite intersection with $I\setminus S$: a finite intersection would imply $S\in F$ after intersecting $A$ with a suitable cofinite set. Hence adjoining $I\setminus S$ generates a free proper filter, which extends to a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) by the [ultrafilter lemma](../../../../../ultrafilter-lemma.md).

Induction on formulas now gives $F\Vdash\phi(\mathbf a)\iff S_\phi(\mathbf a)\in F$. Negation and implication follow by adjoining the positive set on which their classical truth conditions fail. For disjunction, membership of $S_\phi\cup S_\psi$ lets every extension be refined to an ultrafilter containing one of the two sets. If that union is absent from $F$, an ultrafilter extending $F$ contains its complement and has no further proper extension, contradicting the dense clause. For existence, choose coordinate witnesses on $S_{\exists x\phi}$ as in [Łoś theorem](../../../../../los-theorem.md). For universality, if $S_{\forall x\phi}\notin F$, choose a counterexample in every factor outside it and arbitrary elements elsewhere. The resulting sequence has $S_\phi\subseteq S_{\forall x\phi}$, so $F$ cannot force that instance. The converse follows from upward closure and persistence.

At the designated world, therefore,

$$
\boxed{\mathfrak M_I\Vdash\phi\iff S_\phi\text{ is cofinite}\iff\forall\mathcal U\text{ nonprincipal}\;\prod_i\mathfrak M_i/\mathcal U\models\phi.}
$$

This semantics validates **classical first-order logic**, including [law of excluded middle](../../../../../law-of-excluded-middle.md). For example, every free filter has an ultrafilter refinement deciding an atomic formula, so its excluded middle is forced even when neither disjunct is forced at the original world. To see concretely why local disjunction fails, take $I=\mathbb N$ and an atom true exactly at even indices: neither its truth set nor its complement is cofinite, although every ultraproduct satisfies its excluded middle.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
