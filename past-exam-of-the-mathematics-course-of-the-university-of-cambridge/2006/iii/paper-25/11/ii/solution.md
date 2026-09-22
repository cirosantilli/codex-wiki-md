<h1 id="11/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [bounded successor characterization of finite ordinals](../../../../../../bounded-successor-characterization-of-finite-ordinals.md). Let $\operatorname{Ord}(x)$ assert that $x$ is transitive, each of its members is transitive, and any two members are equal or comparable by membership. This is a bounded [first-order formula](../../../../../../first-order-formula.md); [foundation](../../../../../../axiom-of-regularity.md) makes its linear membership order well-founded, so it is precisely the [Von Neumann ordinal](../../../../../../ordinal.md) predicate. Define

$$
\operatorname{Succ}_0(x)\quad\Longleftrightarrow\quad
x=\varnothing\ \lor\ (\exists y\in x)(\forall z\in x)(z=y\ \lor\ z\in y),
$$

and put

$$
\boxed{\operatorname{Nat}(x)\quad\Longleftrightarrow\quad
\operatorname{Ord}(x)\ \land\ \operatorname{Succ}_0(x)\ \land\
(\forall y\in x)\operatorname{Succ}_0(y).}
$$

For an [ordinal](../../../../../../ordinal.md), having a greatest member $y$ says exactly $x=y\cup\{y\}$. The displayed definition makes no reference to an infinite [inductive set](../../../../../../inductive-set.md) or to $\omega$; all quantifiers are bounded within the candidate and its members. Occurrences of $x=\varnothing$ can also be expressed as $(\forall u\in x)\,u\ne u$, so no unbounded quantifier is hidden in empty-set notation.

Every usual [natural number](../../../../../../natural-number.md) satisfies this predicate, by induction: it is a [finite ordinal](../../../../../../finite-ordinal.md), and every nonzero initial segment is a successor. Conversely, suppose an [ordinal](../../../../../../ordinal.md) $x$ is not a usual [natural number](../../../../../../natural-number.md). [Ordinal](../../../../../../ordinal.md) comparability gives $x\ge\omega$. If $x=\omega$, it has no greatest member, contradicting $\operatorname{Succ}_0(x)$. If $x>\omega$, then $\omega\in x$ has no greatest member, contradicting the corresponding bounded requirement on members of $x$. Hence $\operatorname{Nat}(x)$ holds exactly for the usual [natural numbers](../../../../../../natural-number.md). The [axiom of infinity](../../../../../../axiom-of-infinity.md) and [separation](../../../../../../axiom-schema-of-specification.md) therefore collect this class as the usual [set](../../../../../../set-split.md) $\omega$. This is a bounded definition of membership in the natural-number class; it does not claim that the [infinite set](../../../../../../infinite-set.md) $\omega$ itself can be produced without the [infinity](../../../../../../infinity.md) axiom.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11](../../11.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
