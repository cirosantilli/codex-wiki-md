<h1 id="a/4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $S_1$ to consist of the three usual [first-order sentences](../../../../../first-order-sentence.md)

$$
\forall x\ E(x,x),\qquad
\forall x\forall y\,(E(x,y)\to E(y,x)),\qquad
\forall x\forall y\forall z\,((E(x,y)\wedge E(y,z))\to E(x,z)).
$$

These assert [reflexivity](../../../../../reflexive-relation.md), [symmetry](../../../../../symmetry-physics.md) and [transitivity](../../../../../transitive-relation.md) and therefore define exactly the [equivalence relations](../../../../../equivalence-relation.md).

For $S_2$, adjoin to $S_1$ the single [first-order sentence](../../../../../first-order-sentence.md)

$$
\forall x\exists y\,[y\ne x\wedge E(x,y)\wedge
\forall z\,(E(x,z)\to(z=x\vee z=y))].
$$

Its witness $y$ gives a second member of each class, while its final universal clause excludes all others. Hence every class has exactly two members, and conversely such a relation satisfies it. This remains a [finite set](../../../../../finite-set.md) of [first-order sentences](../../../../../first-order-sentence.md).

For each positive [integer](../../../../../integer-split.md) $n$, write

$$
\theta_n(x)=\exists y_1\cdots\exists y_n
\left(\bigwedge_{i=1}^n E(x,y_i)\wedge
\bigwedge_{1\le i<j\le n}y_i\ne y_j\right).
$$

Then

$$
\boxed{S_3=S_1\cup\{\forall x\,\theta_n(x):n\ge1\}.}
$$

Every class in a [first-order model](../../../../../model-of-a-first-order-theory.md) has at least $n$ elements for every $n$, so cannot be finite. Conversely every infinite [equivalence class](../../../../../equivalence-class.md) supplies each finite collection of distinct witnesses. The displayed infinite scheme therefore has exactly the requested [first-order models](../../../../../model-of-a-first-order-theory.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [A](../../../a.md)
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
