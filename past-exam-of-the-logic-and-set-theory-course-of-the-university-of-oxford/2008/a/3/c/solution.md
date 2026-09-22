<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the following [group axioms](../../../../../group-axioms.md) in the given language:

$$
\forall x\forall y\forall z\ ((x+y)+z=x+(y+z)),\qquad
\forall x\forall y\ (x+y=y+x),
$$



$$
\forall x\ (x+0=x),\qquad \forall x\exists y\ (x+y=0).
$$

[Commutativity](../../../../../commutativity.md) supplies the other identity and inverse equations. These [first-order sentences](../../../../../first-order-sentence.md) therefore specify precisely an [abelian group](../../../../../abelian-group.md) with the named identity $0$; an inverse [function symbol](../../../../../function-symbol.md) is unnecessary because inverses are asserted to exist by a [quantified formula](../../../../../quantified-formula.md).

For each positive [integer](../../../../../integer-split.md) $n$, let $t_n(x)$ be the [first-order term](../../../../../first-order-term.md) recursively defined by $t_1(x)=x$ and $t_{n+1}(x)=t_n(x)+x$. Add the [torsion-free abelian group axiom scheme](../../../../../torsion-free-abelian-group-axiom-scheme.md)

$$
\boxed{\forall x\ (t_n(x)=0\to x=0)\qquad(n=1,2,3,\ldots).}
$$

Every [first-order model](../../../../../model-of-a-first-order-theory.md) of these [first-order sentences](../../../../../first-order-sentence.md) is an [abelian group](../../../../../abelian-group.md) with no nonidentity element of [finite order](../../../../../finite-order.md). Conversely every [torsion-free abelian group](../../../../../torsion-free-abelian-group.md) satisfies each of the displayed [first-order sentences](../../../../../first-order-sentence.md). This is a countably infinite first-order axiomatization of exactly the required class.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
