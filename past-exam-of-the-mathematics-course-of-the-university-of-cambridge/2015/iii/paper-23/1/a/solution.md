<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R=\prod_i\mathcal M_i/F$ be the [reduced product](../../../../../../reduced-product.md) by a proper [filter on a set](../../../../../../filter-set-theory.md). Its underlying [equivalence relation](../../../../../../equivalence-relation.md) is $f\sim g$ when $\{i:f(i)=g(i)\}\in F$. Operations are interpreted coordinatewise, and a relation holds of the classes exactly when its coordinate truth set belongs to $F$.

Evaluation of a [first-order term](../../../../../../first-order-term.md) commutes with passage to the quotient, by [mathematical induction](../../../../../../mathematical-induction.md) on terms. Consequently the desired equivalence holds for every [atomic formula](../../../../../../atomic-formula.md), including [logical equality](../../../../../../logical-equality.md). For a formula $\theta$ and representatives $\bar f$, write $S_\theta=\{i:\mathcal M_i\models\theta(\bar f(i))\}$.

For [logical conjunction](../../../../../../logical-conjunction.md), $S_{\theta\wedge\psi}=S_\theta\cap S_\psi$. The [filter on a set](../../../../../../filter-set-theory.md) axioms give

$$
S_\theta\cap S_\psi\in F\quad\Longleftrightarrow\quad S_\theta\in F\text{ and }S_\psi\in F.
$$

Thus the induction hypothesis transfers a conjunction in both directions.

For [existential quantification](../../../../../../existential-quantification.md), first suppose $R\models\exists y\,\theta(y,[\bar f])$. Choose a representative $g$ of a witness. Induction gives $S_{\theta(g,\bar f)}\in F$, and this set is contained in $S_{\exists y\theta}$. Upward closure therefore gives $S_{\exists y\theta}\in F$.

Conversely, suppose $A=S_{\exists y\theta}\in F$. For each $i\in A$, choose a coordinate witness $g(i)$, and choose an arbitrary element of $M_i$ outside $A$. These simultaneous choices use the [axiom of choice](../../../../../../axiom-of-choice.md), as does the usual product construction. Then $A\subseteq S_{\theta(g,\bar f)}$, so that truth set belongs to $F$. Induction gives $R\models\theta([g],[\bar f])$, providing the required witness. Therefore

$$
\boxed{R\models\varphi([\bar f])\iff\{i:\mathcal M_i\models\varphi(\bar f(i))\}\in F}
$$

for every [primitive positive formula](../../../../../../primitive-positive-formula.md). The exam's [tame formulas](../../../../../../primitive-positive-formula.md) are exactly this fragment, built using [logical conjunction](../../../../../../logical-conjunction.md) and [existential quantification](../../../../../../existential-quantification.md). No [ultrafilter](../../../../../../ultrafilter.md) dichotomy was used.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
