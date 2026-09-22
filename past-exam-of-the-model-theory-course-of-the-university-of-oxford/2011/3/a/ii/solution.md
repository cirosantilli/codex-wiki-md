<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here fixed means **fixed setwise**: $\sigma[D]=D$ for every [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md) $\sigma$, not that each point must be fixed individually. A parameter-free [definable set](../../../../../definable-set.md) has this invariance by [automorphism invariance of parameter-free definability](../../../../../automorphism-invariance-of-parameter-free-definability.md).

For the converse, first establish the needed [saturation implies homogeneity](../../../../../saturation-implies-homogeneity.md) step. In a countable [omega-saturated model](../../../../../omega-saturated-model.md), a finite [partial elementary map](../../../../../partial-elementary-map.md) can be extended to include any prescribed additional element in its domain. Transfer the element's [complete type](../../../../../complete-type.md) over the old finite domain along the map. Each finite part of this transported type has a witness because the old map is elementary; the [omega-saturated model](../../../../../omega-saturated-model.md) realizes the full transported type. The inequalities in the type maintain injectivity. Apply the same construction to the inverse map to enlarge the range. Alternating these steps through an enumeration of the countable domain is the [back-and-forth method](../../../../../back-and-forth-method.md), giving a [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md). In particular, any two elements with the same [complete type](../../../../../complete-type.md) over the empty set are related by a [structure automorphism](../../../../../automorphism-of-a-first-order-structure.md).

Assume now that $D$ is finite and invariant, and fix $a\in D$. All realizations in $A$ of $p_a=\operatorname{tp}(a/\varnothing)$ belong to $D$, by the preceding homogeneity and the invariance assumption. Suppose that no parameter-free [first-order formula](../../../../../first-order-formula.md) $\theta_a\in p_a$ has all its realizations in $D$. Then every finite subset of

$$
p_a(x)\cup\{x\ne d:d\in D\}
$$

is satisfiable in $A$: conjoin the finitely many [first-order formulas](../../../../../first-order-formula.md) from $p_a$, and use the assumed absence of a defining neighbourhood inside $D$ to find a witness outside $D$. This is a [partial type](../../../../../partial-type.md) over the finite parameter set $D$. The [omega-saturated model](../../../../../omega-saturated-model.md) would realize it by an element outside $D$ with the same empty-set type as $a$, a contradiction. Hence such a $\theta_a$ does exist.

There are only finitely many $a\in D$, so

$$
\boxed{D=\{x\in A:\mathcal A\models\bigvee_{a\in D}\theta_a(x)\}.}
$$

For $D=\varnothing$, use $x\ne x$. Thus [finite invariant sets in a countable saturated structure are definable](../../../../../finite-invariant-sets-in-a-countable-saturated-structure-are-definable.md). Finiteness is used twice: the extra parameters form a finite set, and the final disjunction is a [first-order formula](../../../../../first-order-formula.md) rather than an infinite disjunction.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the model theory course of the University of Oxford](../../../../split.md)
6. [Model theory course of the University of Oxford](../../../../../model-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
