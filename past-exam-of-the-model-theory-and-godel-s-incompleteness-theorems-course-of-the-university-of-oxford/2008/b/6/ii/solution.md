<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $\mathcal A\subseteq\mathcal B$, interpret each new constant $c_a$ in $\mathcal B$ as the same element $a$. Atomic [logical formulas](../../../../../logical-formula.md) and their [negations](../../../../../negation.md) then have exactly their [truth values](../../../../../truth-value.md) in $\mathcal A_A$, so the expansion satisfies the [diagram of a structure](../../../../../diagram-mathematical-logic.md). If the inclusion is elementary, every [logical formula](../../../../../logical-formula.md) with those named parameters has the same [truth value](../../../../../truth-value.md), so the expansion satisfies the [elementary diagram](../../../../../elementary-diagram-of-a-structure.md).

Conversely, from any expansion $\mathcal B^+$ satisfying the [diagram of a structure](../../../../../diagram-mathematical-logic.md) define

$$
e:A\to B,\qquad e(a)=c_a^{\mathcal B^+}.
$$

The [diagram of a structure](../../../../../diagram-mathematical-logic.md) contains $c_a\ne c_{a'}$ whenever $a\ne a'$, so $e$ is [injective](../../../../../injective-function.md). It contains every true function-value equation, so $e$ commutes with all operations and constants. Positive and negative relation instances ensure both preservation and reflection of the relations. Thus $e$ is an [embedding of first-order structures](../../../../../embedding-of-first-order-structures.md). If the expansion satisfies the [elementary diagram](../../../../../elementary-diagram-of-a-structure.md), for every [logical formula](../../../../../logical-formula.md) $\phi$ and [tuple](../../../../../finite-tuple.md) $\vec a$ it also gives

$$
\mathcal A\models\phi(\vec a)\quad\Longleftrightarrow\quad
\mathcal B\models\phi(e(\vec a)),
$$

so $e$ is an elementary [embedding of first-order structures](../../../../../embedding-of-first-order-structures.md).

**The precise conclusion for an arbitrary expansion is an [embedding of first-order structures](../../../../../embedding-of-first-order-structures.md), rather than a literal inclusion of the original carriers.** The source's inclusion notation is correct when one uses the customary identification of $\mathcal A$ with its embedded copy, or requires the expansion to interpret $c_a$ as the actual element $a$ of a carrier already containing $A$. With that naming convention, $e$ is the inclusion and the requested two equivalences follow exactly.

Without the convention the literal wording fails, even in the [first-order language](../../../../../first-order-language.md) of [logical equality](../../../../../logical-equality.md): singleton [first-order structures](../../../../../first-order-structure.md) with carriers $\{0\}$ and $\{1\}$ have a diagram-satisfying expansion by sending the first [first-order structure](../../../../../first-order-structure.md)'s named point to $1$, but the first carrier is not a [subset](../../../../../subset.md) of the second. The [embedding of first-order structures](../../../../../embedding-of-first-order-structures.md) formulation proved above states the invariant result and makes the intended inclusion formulation precise.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
