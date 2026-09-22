<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [axiom of infinity](../../../../../axiom-of-infinity.md) asserts that an [inductive set](../../../../../inductive-set.md) exists: some [set](../../../../../set-split.md) $I$ contains $0=\varnothing$ and contains $x^+=x\cup\{x\}$ whenever it contains $x$. Inside one such $I$, [axiom of separation](../../../../../axiom-schema-of-specification.md) defines

$$
\omega=\{x\in I:x\text{ belongs to every inductive subset of }I\}.
$$

This [intersection](../../../../../set-intersection.md) is itself inductive and is contained in every [inductive set](../../../../../inductive-set.md), by intersecting that [set](../../../../../set-split.md) with $I$. It is therefore the [set](../../../../../set-split.md) of [natural numbers](../../../../../natural-number.md). If a property holds at $0$ and passes from $n$ to $n^+$, [axiom of separation](../../../../../axiom-schema-of-specification.md) forms the [subset](../../../../../subset.md) of $\omega$ on which it holds. That [subset](../../../../../subset.md) is inductive, so must equal $\omega$. This proves [mathematical induction](../../../../../mathematical-induction.md), including properties with [set](../../../../../set-split.md) parameters.

[Recursion](../../../../../recursion-computer-science.md) on $\omega$ defines the arithmetic operations by

$$
m+0=m,\qquad m+n^+=(m+n)^+,\qquad
m\cdot0=0,\qquad m\cdot n^+=m\cdot n+m.
$$

Existence and uniqueness follow from the [recursion theorem on the natural numbers](../../../../../recursion-theorem-on-the-natural-numbers.md).

For [associativity](../../../../../associative-property.md) of [addition](../../../../../addition.md) fix $m,n$ and induct on $k$. At $k=0$ both sides equal $m+n$. If the equality holds at $k$, then

$$
m+(n+k^+)=m+(n+k)^+=(m+(n+k))^+
=((m+n)+k)^+=(m+n)+k^+.
$$

Thus

$$
\boxed{m+(n+k)=(m+n)+k.}
$$

Every step after the [induction hypothesis](../../../../../induction-hypothesis.md) is a defining successor equation, so [commutativity](../../../../../commutativity.md) has not been used prematurely.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
