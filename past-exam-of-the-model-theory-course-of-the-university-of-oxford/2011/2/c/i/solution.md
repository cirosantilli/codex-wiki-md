<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write

$$
S(x):=\forall y(E(x,y)\to y=x),\qquad R(x):=\exists y(E(x,y)\land y\ne x).
$$

These are [first-order formulas](../../../../../first-order-formula.md) in the original language, not new predicate symbols. An axiomatization consists of the [equivalence relation](../../../../../equivalence-relation.md) axioms for $E$, the bound

$$
\forall x\forall y\forall z\bigl((E(x,y)\land E(x,z))\to(y=z\lor y=x\lor z=x)\bigr),
$$

and, for every $n\geq1$, the two sentences

$$
\exists x_1\cdots x_n\left(\bigwedge_iS(x_i)\land\bigwedge_{i<j}x_i\ne x_j\right),
$$



$$
\exists x_1\cdots x_n\left(\bigwedge_iR(x_i)\land\bigwedge_{i<j}\neg E(x_i,x_j)\right).
$$

The first scheme supplies infinitely many singleton classes. The second supplies infinitely many distinct non-singleton classes; the size bound makes these doubletons.

Every countable [first-order model](../../../../../model-of-a-first-order-theory.md) has countably infinitely many classes of each size. A bijection between singleton classes, and another between doubleton classes followed by a bijection inside each matched pair, gives an [isomorphism](../../../../../isomorphism.md) between any two countable [first-order models](../../../../../model-of-a-first-order-theory.md). To infer completeness, suppose a sentence had different truth values in two arbitrary [first-order models](../../../../../model-of-a-first-order-theory.md). The [Downward Lowenheim-Skolem theorem](../../../../../downward-lowenheim-skolem-theorem.md) supplies countable [elementary substructures](../../../../../elementary-substructure.md) of those [first-order models](../../../../../model-of-a-first-order-theory.md), which would still disagree on the sentence, contradicting the [isomorphism](../../../../../isomorphism.md) just constructed. Thus all [first-order models](../../../../../model-of-a-first-order-theory.md) satisfy the same sentences. Since the original [first-order structure](../../../../../first-order-structure.md) satisfies the axioms, **these axioms form a complete axiomatization of its [first-order theory](../../../../../first-order-theory.md)**. This is the [theory of infinitely many singleton and doubleton equivalence classes](../../../../../theory-of-infinitely-many-singleton-and-doubleton-equivalence-classes.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
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
