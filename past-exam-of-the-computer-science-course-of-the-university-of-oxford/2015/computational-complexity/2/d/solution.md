<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Entail is [co-NP](../../../../../co-np.md)-complete under [polynomial-time many-one reductions](../../../../../polynomial-time-many-one-reduction.md).** For valid [propositional formulas](../../../../../propositional-formula.md), [semantic entailment](../../../../../semantic-entailment.md) holds exactly when the [logical conjunction](../../../../../logical-conjunction.md) of the premise and the conclusion's [logical negation](../../../../../negation.md) is an [unsatisfiable Boolean formula](../../../../../unsatisfiable-boolean-formula.md):

$$
\varphi\models\psi
\quad\Longleftrightarrow\quad
\varphi\land\neg\psi\text{ is unsatisfiable}.
$$

A counterexample to [semantic entailment](../../../../../semantic-entailment.md) is a [Boolean valuation](../../../../../boolean-valuation.md) making $\varphi$ true and $\psi$ false. Guessing one [bit](../../../../../bit.md) for each distinct [Boolean variable](../../../../../boolean-variable.md) and evaluating both [propositional formulas](../../../../../propositional-formula.md) is a [polynomial-time algorithm](../../../../../polynomial-time-algorithm.md). Thus the [complement](../../../../../complement-of-a-set.md) of Entail belongs to [NP](../../../../../np-complexity.md). Malformed descriptions, also in that [complement](../../../../../complement-of-a-set.md), can be accepted after a deterministic syntax check. Hence Entail belongs to [co-NP](../../../../../co-np.md) as a [formal language](../../../../../formal-language.md) over all [strings](../../../../../string.md).

For hardness, the [unsatisfiable Boolean formula](../../../../../unsatisfiable-boolean-formula.md) problem is [co-NP](../../../../../co-np.md)-hard: if $A\in\mathrm{co\text{-}NP}$, then $\overline A\in\mathrm{NP}$, and the permitted [NP-hardness](../../../../../np-hardness.md) of [SAT](../../../../../boolean-satisfiability-problem.md) supplies a [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md) $r$ with

$$
x\in\overline A\quad\Longleftrightarrow\quad r(x)\in\mathrm{SAT}.
$$

We may ensure $r(x)$ is always a valid [propositional formula](../../../../../propositional-formula.md), replacing any malformed output by a fixed contradiction. It follows that $x\in A$ exactly when $r(x)$ is unsatisfiable. This justifies using the unsatisfiability problem as a hardness source without an extra assumption.

Map a valid [propositional formula](../../../../../propositional-formula.md) $\theta$ to

$$
f(\theta)=\langle\theta,\ p\land\neg p\rangle,
$$

where $p$ is a fixed [Boolean variable](../../../../../boolean-variable.md). The second [propositional formula](../../../../../propositional-formula.md) is false under every [Boolean valuation](../../../../../boolean-valuation.md). Consequently it is entailed by $\theta$ precisely when no [Boolean valuation](../../../../../boolean-valuation.md) satisfies $\theta$. Thus

$$
\theta\text{ unsatisfiable}
\quad\Longleftrightarrow\quad f(\theta)\in\mathrm{Entail}.
$$

The output has only constant additional length and is computable in [polynomial time](../../../../../polynomial-time.md). If the source unsatisfiability language rejects malformed [strings](../../../../../string.md), map them to the fixed no-instance $\langle p,p\land\neg p\rangle$. This completes a total [polynomial-time many-one reduction](../../../../../polynomial-time-many-one-reduction.md) and proves the claimed [co-NP](../../../../../co-np.md)-completeness.

$$
\boxed{\mathrm{Entail}\text{ is co-NP-complete}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
