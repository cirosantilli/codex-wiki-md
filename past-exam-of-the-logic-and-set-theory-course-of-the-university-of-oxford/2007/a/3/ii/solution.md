<h1 id="a/3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For independence, construct four [first-order structures](../../../../../first-order-structure.md), each satisfying exactly the three required remaining [axioms](../../../../../axiom.md) and failing the chosen one.

To fail [associativity](../../../../../associative-property.md), use the carrier $\{0,1,2\}$, interpret $c$ as $0$, and define the commutative operation by its table:

$$
\begin{array}{c|ccc}
F&0&1&2\\\hline
0&0&1&2\\
1&1&0&1\\
2&2&1&0
\end{array}
$$

The first row and column give a two-sided identity, and every element is its own inverse because the diagonal entries are $0$. [Symmetry](../../../../../symmetry-physics.md) gives [commutativity](../../../../../commutativity.md). But

$$
F(F(1,1),2)=2\ne0=F(1,F(1,2)),
$$

so [associativity](../../../../../associative-property.md) fails.

To fail the identity axiom, take $\{0,1\}$, $c=0$, and the constant operation $F(x,y)=0$. It is associative and commutative, and every element has a two-sided partner producing $c$; but $F(1,c)=0\ne1$.

To fail the inverse axiom, use [natural numbers](../../../../../natural-number.md) under [addition](../../../../../addition.md) with $c=0$. [Addition](../../../../../addition.md) is associative and commutative and has the required identity, but $1$ has no additive inverse in this carrier.

To fail [commutativity](../../../../../commutativity.md), use the [symmetric group](../../../../../symmetric-group.md) $S_3$ under [permutation](../../../../../permutation.md) composition with $c$ its identity. [Associativity](../../../../../associative-property.md), identity and inverses are [group](../../../../../group-split.md) properties, while $(12)(23)\ne(23)(12)$. Each countermodel witnesses the failure of [semantic entailment](../../../../../semantic-entailment.md) from the other three to the failed [first-order sentence](../../../../../first-order-sentence.md). Hence **the four source [axioms](../../../../../axiom.md) are independent**.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
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
