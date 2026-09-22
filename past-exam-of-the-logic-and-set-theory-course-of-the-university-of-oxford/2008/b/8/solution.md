<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

[Hartogs theorem](../../../../hartogs-theorem.md) says that for every [set](../../../../set-split.md) $X$ there is a least [ordinal](../../../../ordinal-split.md) $h(X)$ for which no [injection](../../../../injective-function.md) $h(X)\to X$ exists. This does not require the [axiom of choice](../../../../axiom-of-choice.md). Form the [set](../../../../set-split.md) $W$ of [well-orderings](../../../../well-order.md) of [subsets](../../../../subset.md) of $X$. It can be defined by the [axiom schema of specification](../../../../axiom-schema-of-specification.md) inside

$$
\mathcal P(X)\times\mathcal P(X\times X),
$$

recording a [subset](../../../../subset.md) and its [well-order](../../../../well-order.md). Each member of $W$ has a unique [ordinal](../../../../ordinal-split.md) [order type](../../../../order-type.md). **[Axiom schema of replacement](../../../../axiom-schema-of-replacement.md) is used to collect those order types into a [set](../../../../set-split.md)**

$$
H=\{\operatorname{otp}(Y,R):(Y,R)\in W\}.
$$

Every member of an [ordinal](../../../../ordinal-split.md) in $H$ is the [order type](../../../../order-type.md) of an initial segment of the corresponding [well-ordering](../../../../well-order.md), so also belongs to $H$. Thus $H$ is a [transitive set](../../../../transitive-set.md) of [ordinals](../../../../ordinal-split.md) and is itself an [ordinal](../../../../ordinal-split.md). An [ordinal](../../../../ordinal-split.md) $\alpha$ belongs to $H$ exactly when it injects into $X$: use a [bijection](../../../../bijection.md) to a [well-ordered](../../../../well-order.md) [subset](../../../../subset.md) in one direction, and transport the [ordinal](../../../../ordinal-split.md) order along the [injection](../../../../injective-function.md) in the other. If $H$ injected into $X$, this characterization would give $H\in H$, impossible for an [ordinal](../../../../ordinal-split.md). All smaller [ordinals](../../../../ordinal-split.md) lie in $H$ and do inject into $X$. Therefore $H=h(X)$. Apart from the standard order-type theorem, the explicit collection of all order types is the [Axiom schema of replacement](../../../../axiom-schema-of-replacement.md) step; no [axiom of choice](../../../../axiom-of-choice.md) of a representative ordering for each type is needed.

[Zorn's lemma](../../../../zorn-s-lemma.md) states that a nonempty [partially ordered set](../../../../partially-ordered-set.md) in which every [chain](../../../../chain-in-a-partial-order.md) has an [upper bound](../../../../upper-bound-in-a-partially-ordered-set.md) has a [maximal element](../../../../maximal-element-of-a-partially-ordered-set.md). Use the [Hartogs bound on partial ordinal injections](../../../../hartogs-bound-on-partial-ordinal-injections.md) to obtain a set-sized [partially ordered set](../../../../partially-ordered-set.md). Consider the partial [injections](../../../../injective-function.md) into $X$ whose domains are [ordinals](../../../../ordinal-split.md). [Hartogs theorem](../../../../hartogs-theorem.md) bounds every such domain strictly below $h=h(X)$. Their [graphs of a function](../../../../graph-of-a-function.md) therefore form a [set](../../../../set-split.md)

$$
P=\{f\subseteq h\times X:f\text{ is an injective function and }\operatorname{dom}f\text{ is an ordinal}\},
$$

obtained by the [axiom schema of specification](../../../../axiom-schema-of-specification.md) from $\mathcal P(h\times X)$. Order $P$ by extension. It is nonempty because it contains the empty [function](../../../../function-split.md). A [chain](../../../../chain-in-a-partial-order.md) has as an [upper bound](../../../../upper-bound-in-a-partially-ordered-set.md) the [union](../../../../set-union.md) of its [graphs of a function](../../../../graph-of-a-function.md): extension makes this a [function](../../../../function-split.md), [injectivity](../../../../injective-function.md) is preserved, and its domain is an [union](../../../../set-union.md) of [ordinals](../../../../ordinal-split.md) and hence an [ordinal](../../../../ordinal-split.md). Its range is contained in $X$, so [Hartogs theorem](../../../../hartogs-theorem.md) forces its domain to be strictly below $h$; thus it belongs to $P$. The empty [chain](../../../../chain-in-a-partial-order.md) also has the empty [function](../../../../function-split.md) as an [upper bound](../../../../upper-bound-in-a-partially-ordered-set.md).

By [Zorn's lemma](../../../../zorn-s-lemma.md) choose a maximal $f:\alpha\to X$. If an element $x\in X$ lay outside its range, appending $f(\alpha)=x$ would give a larger [injection](../../../../injective-function.md) on $\alpha+1$. Such an [injection](../../../../injective-function.md) itself guarantees $\alpha+1<h$ by [Hartogs theorem](../../../../hartogs-theorem.md), so it is a legitimate member of $P$, contradicting [maximality in a partially ordered set](../../../../maximality-in-a-partially-ordered-set.md). Therefore $f$ is [surjective](../../../../surjective-function.md), and

$$
\boxed{X\text{ is equinumerous with an ordinal}.}
$$

For this single extension one only selects an element of one specified nonempty [set](../../../../set-split.md); no additional simultaneous choices are hidden in the argument. [Zorn's lemma](../../../../zorn-s-lemma.md) is the form of the [axiom of choice](../../../../axiom-of-choice.md) used to obtain [maximality in a partially ordered set](../../../../maximality-in-a-partially-ordered-set.md).

Finally work with [cardinals](../../../../cardinal-number-split.md), represented by initial [ordinals](../../../../ordinal-split.md), and put $\mu=\max(\kappa,\lambda)$. It is infinite by hypothesis. Nonzeroness of each factor gives an [injection](../../../../injective-function.md) of the larger [cardinal](../../../../cardinal-number-split.md) into the [Cartesian product](../../../../cartesian-product.md) by holding a coordinate of the other fixed. The supplied infinite-ordinal square result gives $|\mu\times\mu|=\mu$. Hence

$$
\mu\leq\kappa\lambda\leq|\mu\times\mu|=\mu.
$$

For the sum, use [disjoint union](../../../../disjoint-union.md):

$$
\mu\leq\kappa+\lambda\leq|\mu\times\{0,1\}|\leq|\mu\times\mu|=\mu.
$$

The last [injection](../../../../injective-function.md) exists because $\mu$ is infinite and contains two distinct elements. [Cantor-Schröder-Bernstein theorem](../../../../cantor-schroder-bernstein-theorem.md) turns both pairs of bounds into equalities, proving

$$
\boxed{\kappa+\lambda=\kappa\lambda=\max(\kappa,\lambda).}
$$

These final operations are [cardinal sum](../../../../cardinal-sum.md) and [multiplication](../../../../multiplication.md), measuring disjoint [unions](../../../../set-union.md) and Cartesian products. They are not the noncommutative [ordinal arithmetic](../../../../ordinal-arithmetic.md) considered in question 5.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the logic and set theory course of the University of Oxford](../../../split.md)
5. [Logic and set theory course of the University of Oxford](../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
