<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The assertion is false as printed, even for a satisfiable equality-free [Horn clause](../../../../../horn-clause.md).** The original paper allows an arbitrary [quantifier-free formula](../../../../../quantifier-free-formula.md) $G^*$, so in particular permits negative atoms.[Printed p. 4, Question 3(d), final sentence: the matrix is specified as quantifier-free, without a positivity restriction](../../../../../logic-and-proof-examination-paper-of-the-university-of-oxford-2015.md)

Take a [first-order signature](../../../../../first-order-signature.md) with a constant $a$ and unary predicates $P,Q$, and let

$$
F=\forall x\,[\neg P(x)\lor Q(x)],
\qquad G=\exists x\,\neg P(x).
$$

The matrix of $F$ is a [Horn clause](../../../../../horn-clause.md), and the [Herbrand universe](../../../../../herbrand-universe.md) is the singleton $\{a\}$. The possible [Herbrand models](../../../../../herbrand-model.md) of $F$ assign $(P(a),Q(a))$ the values $(0,0)$, $(0,1)$, or $(1,1)$. Neither ground atom is true in every such [Herbrand model](../../../../../herbrand-model.md), so the paper's intersection construction gives

$$
P^{\mathcal H_F}=Q^{\mathcal H_F}=\varnothing.
$$

Consequently $\mathcal H_F\models G$, with witness $a$. However, the one-element [first-order structure](../../../../../first-order-structure.md) in which both predicates hold everywhere satisfies $F$ and falsifies $G$. Hence

$$
\boxed{\mathcal H_F\models G\quad\text{but}\quad F\not\models G.}
$$

This directly refutes the requested implication; no proof of the stated equivalence is possible. It also isolates the issue: an atom being absent from the intersection means that it is false in _some_ [Herbrand model](../../../../../herbrand-model.md), not that it is false in every [first-order model](../../../../../model-of-a-first-order-theory.md).

The standard correct version assumes that $F$ is satisfiable, uses an equality-free [first-order signature](../../../../../first-order-signature.md) with a nonempty [Herbrand universe](../../../../../herbrand-universe.md), and requires $G^*$ to be a positive [quantifier-free formula](../../../../../quantifier-free-formula.md): one built from atoms and truth constants using only [logical conjunction](../../../../../logical-conjunction.md) and [logical disjunction](../../../../../logical-disjunction.md). Under those assumptions the expected argument is as follows.

First, the intersection of the ground atoms true in all [Herbrand models](../../../../../herbrand-model.md) is itself a [Herbrand model](../../../../../herbrand-model.md) of $F$. To see this, read each ground [Horn clause](../../../../../horn-clause.md) as $A_1\land\cdots\land A_k\to B$, where $B$ is an atom or false. If every $A_i$ is true in the intersection, every $A_i$ is true in every [Herbrand model](../../../../../herbrand-model.md). When $B$ is an atom, all these [Herbrand models](../../../../../herbrand-model.md) must make $B$ true, so the intersection does too. When $B$ is false, the antecedent cannot hold in any [Herbrand model](../../../../../herbrand-model.md); since there is at least one such model, it cannot hold in the intersection either. Thus the intersection is the [least Herbrand model](../../../../../least-herbrand-model.md).

Now let $\mathcal H_F\models G$ for positive $G^*$. There is a tuple of [ground terms](../../../../../ground-term.md) $\bar t$ with $\mathcal H_F\models G^*(\bar t)$. Expand the positive [quantifier-free formula](../../../../../quantifier-free-formula.md) into [disjunctive normal form](../../../../../disjunctive-normal-form.md); one of its [logical conjunctions](../../../../../logical-conjunction.md) of positive atoms is true at $\bar t$. Each of those ground atoms $A$ holds in every [Herbrand model](../../../../../herbrand-model.md) of $F$. It also follows that $F\models A$: otherwise a [first-order model](../../../../../model-of-a-first-order-theory.md) of $F\land\neg A$ would, by [Herbrand's theorem](../../../../../herbrand-s-theorem.md) for universal equality-free [first-order clauses](../../../../../first-order-clause.md), yield a [Herbrand model](../../../../../herbrand-model.md) of $F\land\neg A$, a contradiction. Every [first-order model](../../../../../model-of-a-first-order-theory.md) of $F$ therefore satisfies the same positive [logical conjunction](../../../../../logical-conjunction.md) at the interpretations of $\bar t$, and hence satisfies $G$.

Conversely, if $F\models G$, the fact that the [least Herbrand model](../../../../../least-herbrand-model.md) is a [first-order model](../../../../../model-of-a-first-order-theory.md) of $F$ immediately gives $\mathcal H_F\models G$. Thus the repaired conclusion is

$$
\boxed{\mathcal H_F\models G\ \Longleftrightarrow\ F\models G
\quad\text{for satisfiable universal Horn }F\text{ and positive existential }G.}
$$

The satisfiability qualification is separately necessary when general [Horn clauses](../../../../../horn-clause.md) may have no positive conclusion. For instance, $F=\forall x(P(x)\land\neg P(x))$ is a [logical conjunction](../../../../../logical-conjunction.md) of [Horn clauses](../../../../../horn-clause.md) with no models. The intersection convention then makes every ground atom true by vacuity, yet $F$ entails even $\exists x\neg P(x)$, which that [Herbrand structure](../../../../../herbrand-structure.md) falsifies. The earlier satisfiable example already refutes the printed claim without relying on this further defect.

## ↑ Ancestors (11)

1. [D](../d.md)
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
