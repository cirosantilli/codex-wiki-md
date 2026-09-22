<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [first-order signature](../../../../../first-order-signature.md) with at least one constant symbol, its [Herbrand universe](../../../../../herbrand-universe.md) is the set of all [ground terms](../../../../../ground-term.md) built from its constant and function symbols. If necessary add a fresh constant to make this set nonempty. A [Herbrand structure](../../../../../herbrand-structure.md) has exactly this domain; each constant denotes itself and each function symbol forms the corresponding syntactic [first-order term](../../../../../first-order-term.md). Its remaining choices are the [truth values](../../../../../truth-value.md) of the ground predicate atoms. For example, with constant $a$ and unary function $f$, the [Herbrand universe](../../../../../herbrand-universe.md) is $\{a,f(a),f(f(a)),\ldots\}$.

One useful clausal form of [Herbrand's theorem](../../../../../herbrand-s-theorem.md) is the following. For a set $S$ of universally quantified, equality-free [first-order clauses](../../../../../first-order-clause.md),

$$
\boxed{S\text{ is unsatisfiable}\quad\Longleftrightarrow\quad
\text{some finite set of ground instances of }S\text{ is propositionally unsatisfiable}.}
$$

Ground instances substitute [ground terms](../../../../../ground-term.md) for all variables. On the right, treat the ground predicate atoms as independent [Boolean variables](../../../../../boolean-variable.md). Equivalently, $S$ is satisfiable if and only if it has a [Herbrand model](../../../../../herbrand-model.md). A general [first-order sentence](../../../../../first-order-sentence.md) can first be put into [Skolem normal form](../../../../../skolem-normal-form.md) and [clausal form](../../../../../clausal-form.md), with the new symbols included in the [Herbrand universe](../../../../../herbrand-universe.md).

An equivalent existential version says that a valid equality-free [first-order sentence](../../../../../first-order-sentence.md) $\exists\bar x\,\theta(\bar x)$ with [quantifier-free formula](../../../../../quantifier-free-formula.md) $\theta$ has finitely many ground tuples $\bar t_1,\ldots,\bar t_r$ such that $\bigvee_{i=1}^r\theta(\bar t_i)$ is propositionally valid, adding a constant if needed. This explains why a finite [ground resolution](../../../../../ground-resolution.md) refutation can establish a consequence involving infinitely many possible [ground terms](../../../../../ground-term.md).

The equality-free qualification matters. If [first-order equality](../../../../../logical-equality.md) is present, one must handle its axioms and use a term model modulo a suitable congruence, or use the corresponding theorem with equality. Literal syntactic term interpretation alone cannot model a consistent requirement such as $a=b$ for distinct constant symbols.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
