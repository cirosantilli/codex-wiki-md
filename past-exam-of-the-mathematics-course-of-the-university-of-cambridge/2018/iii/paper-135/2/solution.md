<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the following form of the [omitting types theorem](../../../../../omitting-types-theorem.md). Let $T$ be a [consistent first-order theory](../../../../../consistent-first-order-theory.md) in a countable [first-order language](../../../../../first-order-language.md), and let $(p_j(\mathbf x_j))_{j\in\mathbb N}$ be a countable family of finite-arity [partial types](../../../../../partial-type.md). Suppose each is a [nonprincipal partial type](../../../../../nonprincipal-partial-type.md): no formula $\theta(\mathbf x_j)$ consistent with $T$ satisfies $T\vdash\theta\to\psi$ for every $\psi\in p_j$. Then $T$ has a countable model omitting all the $p_j$.

For the proof, add countably many fresh constants and perform a [Henkin construction](../../../../../henkin-construction.md). Enumerate three kinds of tasks: deciding each sentence, providing a fresh constant witness for each existential sentence, and making every constant tuple omit each $p_j$ of the corresponding arity. Starting with the empty set, keep a finite set $\Gamma_s$ such that $T\cup\Gamma_s$ is consistent. A sentence can be decided in one of its two ways while preserving consistency. For an existential sentence, add $\exists x\,\alpha(x)\to\alpha(c)$ with $c$ fresh; inconsistency would contradict freshness and the existential sentence itself.

For an omission task at a tuple $\mathbf c$, let $\gamma$ be the conjunction of $\Gamma_s$. Replace its constants by variables, identify the occurrences of the tuple's constants with the corresponding variables $\mathbf x$, and existentially quantify the other variables. If the tuple repeats a constant, include the corresponding equalities between its variables. This gives $\theta(\mathbf x)$ with $T\cup\{\exists\mathbf x\,\theta\}$ consistent. Nonprincipality supplies $\psi\in p_j$ such that

$$
T\cup\{\exists\mathbf x\,(\theta\land\neg\psi)\}
$$

is consistent. Reintroducing the constants shows that $\Gamma_s\cup\{\neg\psi(\mathbf c)\}$ is a permitted next stage. Thus each constant tuple will fail some formula of each prescribed type.

The union $T^*=T\cup\bigcup_s\Gamma_s$ is consistent by the finite character of formal proofs, complete in the expanded language, and has the [Henkin witness property](../../../../../henkin-witness-property.md). Its [term model](../../../../../term-model.md) has closed terms modulo provable equality as elements, and satisfies the [truth lemma for a Henkin term model](../../../../../truth-lemma-for-a-henkin-term-model.md), proved by induction on formulas. It is countable. Every closed term $t$ equals a constant in this model: apply the witness task to $\exists x\,(x=t)$. Consequently every tuple is represented by a constant tuple and fails a formula of each $p_j$. This proves simultaneous omission.

For arithmetic, the [nonstandard element type](../../../../../nonstandard-element-type.md) is

$$
p_\infty(x)=\{x>\overline n:n\in\mathbb N\}.
$$

In a model of [Peano arithmetic](../../../../../peano-arithmetic.md), an element omits this type precisely when it is one of the standard numerals: arithmetic proves that every element at most $\overline n$ equals one of $\overline0,\ldots,\overline n$. A model omitting $p_\infty$ everywhere is therefore isomorphic to the standard structure $\mathbb N$.

For a complete consistent theory $T\supseteq\mathrm{PA}$, this gives the particularly useful equivalence

$$
\boxed{p_\infty\text{ nonprincipal over }T\iff T\text{ has a standard model}\iff T=\operatorname{Th}(\mathbb N).}
$$

The first implication is the [omitting types theorem](../../../../../omitting-types-theorem.md). For the converse, if a consistent $\theta$ over the [theory of true arithmetic](../../../../../true-arithmetic.md) implied every $x>\overline n$, completeness would give $\mathbb N\models\exists x\,\theta(x)$. A standard witness $m$ contradicts the implication $\theta\to x>\overline m$.

Completeness matters in this formulation. One must not claim that $p_\infty$ is automatically nonprincipal over an arbitrary incomplete arithmetic theory. For example, assuming consistency of [Peano arithmetic](../../../../../peano-arithmetic.md), the formula saying that $x$ is the least code of a proof of a contradiction is consistent with that theory, by [Gödel second incompleteness theorem](../../../../../godel-second-incompleteness-theorem.md), and implies $x>\overline n$ for each standard $n$. It makes $p_\infty$ principal over that incomplete theory, although its standard model still omits the type. The theorem is a sufficient omission criterion, not a necessary one for arbitrary partial types over incomplete theories.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
