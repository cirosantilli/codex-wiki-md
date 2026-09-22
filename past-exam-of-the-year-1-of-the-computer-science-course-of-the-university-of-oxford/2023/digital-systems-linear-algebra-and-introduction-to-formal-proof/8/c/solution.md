<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Read the initial universal [quantifiers](../../../../../quantifier.md) as governing the conjunction of irreflexivity and transitivity. Explicitly, the intended [first-order sentence](../../../../../first-order-sentence.md) asserts

$$
\forall x\forall y\forall z\bigl(\neg Q(x,x)\land
((Q(x,y)\land Q(y,z))\to Q(x,z))\bigr)
\quad\land\quad\forall x\exists y\,Q(x,y).
$$

Thus $Q$ is an [irreflexive relation](../../../../../irreflexive-relation.md), a [transitive relation](../../../../../transitive-relation.md), and a [serial relation](../../../../../serial-relation.md).

Suppose a [first-order model](../../../../../model-of-a-first-order-theory.md) had a finite nonempty domain of [cardinality](../../../../../cardinality.md) $N$. Choose $a_0$. Seriality supplies successive elements $a_1,\ldots,a_N$ with $Q(a_i,a_{i+1})$. By the [pigeonhole principle](../../../../../pigeonhole-principle.md), $a_i=a_j$ for some $i<j$. Repeated transitivity along that part of the chain gives $Q(a_i,a_j)=Q(a_i,a_i)$, contradicting irreflexivity. Hence **there is no finite nonempty model**. This is the [infinite-model property of a serial strict partial order](../../../../../infinite-model-property-of-a-serial-strict-partial-order.md).

**An infinite model exists:** take domain $\mathbb N$ and $Q(x,y)$ to mean $x<y$. It is irreflexive and transitive, and $y=x+1$ witnesses seriality for every $x$.

The quantifier-scope convention matters: giving each printed universal [quantifier](../../../../../quantifier.md) only the immediately following atomic scope would leave the transitivity implication with [free variables](../../../../../free-variable.md) and would not express the claimed theorem. The explicit parenthesisation above records the reading under which the source's requested assertion is valid.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Introduction to formal proof](../../introduction-to-formal-proof.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
