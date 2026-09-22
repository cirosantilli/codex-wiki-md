<h1 id="b/8/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Adjoin to $T$ the [negations](../../../../../negation.md) of all closed-term instances of $\theta$. If the resulting [set](../../../../../set-split.md) had a [first-order model](../../../../../model-of-a-first-order-theory.md) $\mathcal A$, its [ground-term substructure](../../../../../ground-term-substructure.md) $\mathcal B$ from (ii) would still [first-order model](../../../../../model-of-a-first-order-theory.md) $T$. The assumed existential consequence therefore supplies a [tuple](../../../../../finite-tuple.md) $\vec b$ in $\mathcal B$ satisfying $\theta$. Each $b_j$ is the value of a [closed term](../../../../../closed-term.md) $t_j$.

Quantifier-free agreement between a [substructure](../../../../../substructure-of-a-first-order-structure.md) and its ambient [first-order structure](../../../../../first-order-structure.md) gives

$$
\mathcal A\models\theta(t_1,\ldots,t_k),
$$

contradicting the adjoined [negation](../../../../../negation.md) of this very ground instance. Thus

$$
T\cup\{\neg\theta(t_1,\ldots,t_k):t_1,\ldots,t_k\text{ closed terms}\}
$$

is unsatisfiable. [Compactness theorem](../../../../../compactness-theorem.md) gives a finite unsatisfiable [subset](../../../../../subset.md). Its finitely many ground [negations](../../../../../negation.md) imply that, for some finite list of [first-order term](../../../../../first-order-term.md) [tuples](../../../../../finite-tuple.md),

$$
\boxed{T\models\bigvee_{i=1}^m\theta(t_{i1},\ldots,t_{ik}).}
$$

If the finite [subset](../../../../../subset.md) already shows $T$ itself inconsistent and supplies no ground [negations](../../../../../negation.md), choose any one closed-term [tuple](../../../../../finite-tuple.md) using the available constant; then any [first-order sentence](../../../../../first-order-sentence.md) is a consequence of $T$, so $m=1$ suffices. Otherwise the selected list is nonempty. This also explains why the conclusion contains a finite disjunction rather than necessarily one universal choice of a witness [first-order term](../../../../../first-order-term.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
