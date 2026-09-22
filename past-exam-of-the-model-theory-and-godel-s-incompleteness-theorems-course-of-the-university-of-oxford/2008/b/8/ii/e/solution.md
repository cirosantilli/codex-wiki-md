<h1 id="b/8/ii/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the [first-order theory](../../../../../../first-order-theory.md) $T_{\mathbb Z}$ of a [bijection](../../../../../../bijection.md) $f$ with named inverse $g$ and no finite cycles. Its axioms are

$$
\forall x\ f(g(x))=x,\qquad\forall x\ g(f(x))=x,\qquad
\forall x\ f^n(x)\ne x\quad(n=1,2,3,\ldots).
$$

Every [first-order model](../../../../../../model-of-a-first-order-theory.md) is a disjoint [union](../../../../../../set-union.md) of free two-sided [integer](../../../../../../integer-split.md) orbits. Write $f^k$ for positive powers of $f$ and for powers of $g$ when $k$ is negative.

This [first-order theory](../../../../../../first-order-theory.md) is complete and eliminates [quantifiers](../../../../../../quantifier.md). Every [first-order term](../../../../../../first-order-term.md) reduces to $f^k(x_i)$, and atomic [logical formulas](../../../../../../logical-formula.md) reduce to statements $x_j=f^k(x_i)$. To eliminate an existential [logical variable](../../../../../../logical-variable.md) in a [conjunction](../../../../../../conjunction-astronomy.md) of literals, first remove self-equalities using the no-finite-cycle axioms. If an equation fixes that [logical variable](../../../../../../logical-variable.md) as an [integer](../../../../../../integer-split.md) translate of another [logical variable](../../../../../../logical-variable.md), substitute that value. If no such equation remains, only finitely many points are excluded by the remaining inequalities, so some value exists in the infinite domain. Apply this to [disjunctive normal form](../../../../../../disjunctive-normal-form.md) and then induct on [logical formulas](../../../../../../logical-formula.md). The resulting parameter-free [first-order sentences](../../../../../../first-order-sentence.md) are decided, proving completeness.

For each fixed finite $n$, a [complete type](../../../../../../complete-type.md) records a partition of the [logical variables](../../../../../../logical-variable.md) into common orbits and finitely many [integer](../../../../../../integer-split.md) offsets within each block. There are countably many possibilities. [Countable](../../../../../../countable-set.md) [first-order models](../../../../../../model-of-a-first-order-theory.md) with one orbit and with two orbits are not [isomorphic](../../../../../../isomorphism.md), so the [first-order theory](../../../../../../first-order-theory.md) is not $\aleph_0$-categorical.

Thus this example has the source's explicitly defined countable-type property. In fact it also satisfies ordinary [omega-stability](../../../../../../omega-stability-of-a-theory.md): over a [countable](../../../../../../countable-set.md) parameter [set](../../../../../../set-split.md), an element is either a specified [integer](../../../../../../integer-split.md) translate of a parameter, giving countably many possibilities, or lies in an entirely new orbit, giving one further [complete one-type](../../../../../../complete-one-type.md). The same finite-orbit-pattern description handles finite [tuples](../../../../../../finite-tuple.md). Therefore

$$
\boxed{T_{\mathbb Z}\text{ has countably many }n\text{-types for every finite }n,
\text{ but is not }\aleph_0\text{-categorical}.}
$$

The source prints the label “$0$-stable”; the construction meets its stated definition as well as the usual stronger [omega-stability](../../../../../../omega-stability-of-a-theory.md) condition. The difference between countably many and finitely many [partial types](../../../../../../partial-type.md) is exactly why Ryll-Nardzewski does not yield categoricity here.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [Ii](../../ii.md)
3. [8](../../../8.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../split.md)
7. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
