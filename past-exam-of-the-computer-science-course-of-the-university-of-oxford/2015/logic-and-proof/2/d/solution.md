<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

It suffices to eliminate one [existential quantifier](../../../../../existential-quantification.md) from a [quantifier-free formula](../../../../../quantifier-free-formula.md) $\theta(y,\bar x)$. Indeed, [logical connectives](../../../../../logical-connective.md) preserve equivalence, and a [universal quantifier](../../../../../universal-quantification.md) can be rewritten using $\forall y\,\alpha\equiv\neg\exists y\,\neg\alpha$. An induction on the construction of a [first-order formula](../../../../../first-order-formula.md) then eliminates all its [quantifiers](../../../../../quantifier.md) from the inside out.

Convert $\theta$ to [disjunctive normal form](../../../../../disjunctive-normal-form.md). Since [existential quantification](../../../../../existential-quantification.md) distributes over a finite [logical disjunction](../../../../../logical-disjunction.md), consider a single [logical conjunction](../../../../../logical-conjunction.md) of atomic [first-order formulas](../../../../../first-order-formula.md) and their negations. There are no function or constant symbols in this [first-order signature](../../../../../first-order-signature.md), so its atoms are equalities between variables and instances of $E$ between variables.

For a tuple $\bar x=(x_1,\ldots,x_r)$, enumerate its possible complete atomic diagrams $\delta(\bar x)$. Such a [quantifier-free formula](../../../../../quantifier-free-formula.md) specifies which variables are equal and, between distinct equality classes, exactly which pairs are adjacent. Keep only the diagrams in which [first-order equality](../../../../../logical-equality.md) is an [equivalence relation](../../../../../equivalence-relation.md) and $E$ is symmetric and irreflexive. There are finitely many diagrams for each $r$, and every tuple in a [first-order model](../../../../../model-of-a-first-order-theory.md) of $T$ satisfies exactly one of them. Every retained diagram is realizable: insert one [vertex](../../../../../vertex-graph-theory.md) for each equality class successively, using the extension axioms to prescribe its adjacency to earlier [vertices](../../../../../vertex-graph-theory.md).

Fix one diagram $\delta$. A potential [existential witness](../../../../../existential-witness.md) for $y$ has one of two forms.

- **An existing [vertex](../../../../../vertex-graph-theory.md).** If $y=x_i$, substitute $x_i$ for $y$ in the [logical conjunction](../../../../../logical-conjunction.md). The diagram $\delta$ decides the [truth value](../../../../../truth-value.md) of every resulting atom, and so decides whether this choice works.
- **A new [vertex](../../../../../vertex-graph-theory.md).** Require $y\ne x_i$ for every $i$. Simplify $y=y$ to true and $E(y,y)$ to false. Use symmetry to rewrite every remaining edge requirement involving $y$ in the form $E(x_i,y)$ or $\neg E(x_i,y)$. An equality $y=x_i$, a positive loop requirement, or opposite edge requirements on the same equality class makes this case impossible. Otherwise the requirements give a consistent adjacency pattern on finitely many distinct [vertices](../../../../../vertex-graph-theory.md). Any equality classes without a specified edge requirement can be assigned either pattern. Reorder representatives with the desired neighbours first; the appropriate extension axiom supplies a fresh [vertex](../../../../../vertex-graph-theory.md) with precisely this pattern.

All [first-order formulas](../../../../../first-order-formula.md) involving only $\bar x$ are already decided by $\delta$. Therefore, for each diagram, the existence of a suitable $y$ has a definite answer, determined by a finite syntactic test. Let $\mathcal D$ be the set of diagrams for which at least one disjunct and at least one of the two witness cases succeeds. Then

$$
\boxed{T\models\forall\bar x\left[
\exists y\,\theta(y,\bar x)\leftrightarrow
\bigvee_{\delta\in\mathcal D}\delta(\bar x)\right].}
$$

The right side is a [quantifier-free formula](../../../../../quantifier-free-formula.md). An empty [logical disjunction](../../../../../logical-disjunction.md) means false, and for an empty tuple the empty atomic diagram means true. These logical truth constants also handle closed [first-order sentences](../../../../../first-order-sentence.md) in this constant-free [first-order signature](../../../../../first-order-signature.md).

For a concrete illustration of the fresh-witness case,

$$
T\models\forall x_1\forall x_2\forall x_3\left[
\exists y\,(E(y,x_1)\land\neg E(y,x_2)\land y\ne x_3)
\leftrightarrow x_1\ne x_2\right].
$$

If $x_1=x_2$, the edge requirements conflict. Otherwise the extension property supplies a [vertex](../../../../../vertex-graph-theory.md) outside the finite set of parameters with the desired pattern; the extra avoidance of $x_3$ causes no obstruction. The general diagram construction handles all such equality coincidences systematically and proves [quantifier elimination](../../../../../quantifier-elimination.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
