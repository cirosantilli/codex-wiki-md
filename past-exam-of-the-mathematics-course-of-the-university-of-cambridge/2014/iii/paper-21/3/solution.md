<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Every countable structure in a countable [first-order language](../../../../../first-order-language.md) has a [Scott sentence](../../../../../scott-sentence.md) whose countable models are precisely its [isomorphic](../../../../../isomorphism.md) copies.** In particular two countable structures with the same [countable infinitary logic](../../../../../countable-infinitary-logic.md) sentences are [isomorphic](../../../../../isomorphism.md). Countability of both structures is essential to the back-and-forth conclusion; the sentence need not exclude uncountable models.

Let $M$ be a nonempty countable structure in a countable [first-order language](../../../../../first-order-language.md). The [countable infinitary logic](../../../../../countable-infinitary-logic.md) $L_{\omega_1,\omega}$ permits countable [logical conjunctions](../../../../../logical-conjunction.md) and [logical disjunctions](../../../../../logical-disjunction.md), but only finite strings of quantifiers and finitely many [free variables](../../../../../free-variable.md) in each formula. We construct a [Scott formula](../../../../../scott-formula.md) $\phi_{\bar a}^{\alpha}(\bar x)$ for every finite [tuple](../../../../../finite-tuple.md) $\bar a$ from $M$ and every countable [ordinal](../../../../../ordinal.md) $\alpha$.

At stage zero, let $\phi_{\bar a}^{0}$ be the conjunction of all [atomic formulas](../../../../../atomic-formula.md) true of $\bar a$ and the negations of all [atomic formulas](../../../../../atomic-formula.md) false of $\bar a$. Include atomic formulas involving arbitrary terms and constants, not just relation symbols applied directly to variables. There are only countably many such formulas. This complete atomic description ensures that matching [tuples](../../../../../finite-tuple.md) determine a [partial isomorphism of structures](../../../../../partial-embedding.md).

At successors put

$$
\begin{aligned}
\phi_{\bar a}^{\alpha+1}(\bar x)=\;&\phi_{\bar a}^{\alpha}(\bar x)\\
&\land\bigwedge_{b\in M}\exists y\;\phi_{\bar a,b}^{\alpha}(\bar x,y)\\
&\land\forall y\;\bigvee_{b\in M}\phi_{\bar a,b}^{\alpha}(\bar x,y).
\end{aligned}
$$

At a nonzero limit [ordinal](../../../../../ordinal.md) $\lambda<\omega_1$, put $\phi_{\bar a}^{\lambda}=\bigwedge_{\beta<\lambda}\phi_{\bar a}^{\beta}$. All these are formulas of [countable infinitary logic](../../../../../countable-infinitary-logic.md): each indexing set is countable, and the [free variables](../../../../../free-variable.md) are only the fixed finite [tuple](../../../../../finite-tuple.md). Rename bound variables when necessary. [Transfinite induction](../../../../../transfinite-induction.md) also shows $M\models\phi_{\bar a}^{\alpha}(\bar a)$.

For [tuples](../../../../../finite-tuple.md) of the same length within $M$, define $\bar a\equiv_\alpha\bar b$ by $M\models\phi_{\bar a}^{\alpha}(\bar b)$. Induction identifies this with the usual symmetric [back-and-forth method](../../../../../back-and-forth-method.md) equivalence: the [tuples](../../../../../finite-tuple.md) have the same atomic description at stage zero, and at a successor every one-element extension on either side has a matching extension at the previous stage. Thus these are decreasing [equivalence relations](../../../../../equivalence-relation.md), simultaneously for every finite [tuple](../../../../../finite-tuple.md) length.

There are only countably many pairs of finite [tuples](../../../../../finite-tuple.md) in $M$. A pair can cease to be equivalent at most once. The supremum of the first separation stages of all pairs that separate below $\omega_1$ is a countable [ordinal](../../../../../ordinal.md). Choose a countable $\alpha$ at least that supremum. No pair can first separate at $\alpha+1$, so

$$
\equiv_\alpha\;=\;\equiv_{\alpha+1}\quad\text{on every }M^n.
$$

This justifies stabilization without assuming that all [tuples](../../../../../finite-tuple.md) stabilize at one predetermined finite stage.

Now form the following [Scott sentence](../../../../../scott-sentence.md), where the case $n=0$ has no displayed variables or quantifiers:

$$
\sigma_M=\phi_{\varnothing}^{\alpha}\ \land\
\bigwedge_{n<\omega}\ \bigwedge_{\bar a\in M^n}
\forall\bar x\;\bigl(\phi_{\bar a}^{\alpha}(\bar x)\to\phi_{\bar a}^{\alpha+1}(\bar x)\bigr).
$$

It is a sentence of [countable infinitary logic](../../../../../countable-infinitary-logic.md), because the family of all finite [tuples](../../../../../finite-tuple.md) is countable. The stabilization above and the truth of $\phi_{\varnothing}^{\alpha}$ show $M\models\sigma_M$.

Suppose a countable structure $N$ satisfies $\sigma_M$. Start with the empty matching [tuples](../../../../../finite-tuple.md), and maintain $N\models\phi_{\bar a}^{\alpha}(\bar b)$. The corresponding conjunct of $\sigma_M$ upgrades this to $N\models\phi_{\bar a}^{\alpha+1}(\bar b)$. The existential conjuncts extend the match by any specified element of $M$. The universal-disjunction conjunct extends it by any specified element of $N$. The [atomic formula](../../../../../atomic-formula.md) information makes a new element on one side match a new element on the other, and makes repeated elements agree with their earlier matches.

Enumerate both structures and alternate these two extension steps, including the least element not yet covered at each step. The union is a [bijection](../../../../../bijection.md) preserving and reflecting every [atomic formula](../../../../../atomic-formula.md), hence an [isomorphism](../../../../../isomorphism.md); for function symbols, eventually include both a [tuple](../../../../../finite-tuple.md) and the value of its function term to see explicitly that the function is preserved. For finite structures the same construction stops when both are covered. Conversely every [isomorphic](../../../../../isomorphism.md) copy of $M$ satisfies $\sigma_M$, since [isomorphisms](../../../../../isomorphism.md) preserve formulas of [countable infinitary logic](../../../../../countable-infinitary-logic.md) by induction on their construction. Therefore

$$
\boxed{\text{for countable }N,\qquad N\models\sigma_M\iff N\cong M.}
$$

If countable $M,N$ have the same $L_{\omega_1,\omega}$ sentences, $N$ satisfies this [Scott sentence](../../../../../scott-sentence.md) of $M$ and is [isomorphic](../../../../../isomorphism.md) to $M$. This proves [Scott isomorphism theorem](../../../../../scott-isomorphism-theorem.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
