<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a structure in a [countable](../../../../../countable-set.md) language and any subset $C$ of its domain, there is an [elementary substructure](../../../../../elementary-substructure.md) containing $C$ of [cardinality](../../../../../cardinality.md) at most $\max(|C|,\aleph_0)$. In particular a finite or [countable](../../../../../countable-set.md) $C$ lies in a [countable](../../../../../countable-set.md) [elementary substructure](../../../../../elementary-substructure.md). This is the downward [Löwenheim-Skolem theorem](../../../../../lowenheim-skolem-theorem.md).

Construct it directly inside the given structure $A$. Start with $C_0$ containing $C$, the interpretations of the constants, and one element if needed to ensure a nonempty domain. Given $C_n$, for every formula $\exists x\,\varphi(x,a)$ with its finite parameter tuple from $C_n$ that is true in $A$, choose one actual witness in $A$ and place it in $C_{n+1}$. Retain $C_n$ as well. There are at most $\max(|C|,\aleph_0)$ choices at each stage. Let $B=\bigcup_{n<\omega}C_n$.

The construction closes $B$ under every function of the language: for a tuple in $C_n$, the formula $x=f(a)$ forces its unique value into the next stage. Thus $B$ carries the induced [substructure](../../../../../substructure-of-a-first-order-structure.md), and it has the asserted [cardinal](../../../../../cardinal-number-split.md) bound.

Prove elementarity by [structural induction](../../../../../structural-induction.md). [Atomic formulas](../../../../../atomic-formula.md) agree by the induced-substructure construction; [logical connectives](../../../../../logical-connective.md) preserve agreement. For an existential formula with parameters in $B$, if it is true in $A$, all its parameters occur in some $C_n$, so the chosen witness lies in $C_{n+1}\subseteq B$. The induction hypothesis makes its matrix true in $B$. In the other direction a witness in $B$ is also a witness in $A$, again by induction. This is the [Tarski-Vaught test](../../../../../tarski-vaught-test.md), with its witness argument proved explicitly. No completeness or [compactness theorem](../../../../../compactness-theorem.md) theorem enters the construction.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../split.md)
6. [Model theory and Gödel's incompleteness theorems course of the University of Oxford](../../../../../model-theory-and-godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
