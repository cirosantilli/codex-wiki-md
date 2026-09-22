<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here the [power set](../../../../../../power-set.md) notation gives $xEy\iff\mathcal P(x)\subseteq y$. Suppose a nonempty [set](../../../../../../set-split.md) $A$ has no $E$-minimal member. Form its [intersection](../../../../../../set-intersection.md) $b=\bigcap A$. This is a set: for any one $a_0\in A$, use the [axiom schema of separation](../../../../../../axiom-schema-of-specification.md) inside $a_0$ to define the elements common to all members of $A$. Selecting a single witness to nonemptiness is not an application of the [axiom of choice](../../../../../../axiom-of-choice.md).

For an arbitrary $y\in A$, lack of minimality supplies some $x\in A$ with $\mathcal P(x)\subseteq y$. Since $b\subseteq x$, every [subset](../../../../../../subset.md) of $b$ is a subset of $x$, so

$$
\mathcal P(b)\subseteq\mathcal P(x)\subseteq y.
$$

This conclusion holds for each $y\in A$, without choosing all the corresponding $x$ simultaneously. Intersecting over $y$ gives $\mathcal P(b)\subseteq b$.

For completeness, the contradiction in [Cantor's theorem](../../../../../../cantor-s-theorem.md) is completely explicit here. By the [axiom schema of separation](../../../../../../axiom-schema-of-specification.md) put $d=\{u\in b:u\notin u\}$. Then $d\in\mathcal P(b)\subseteq b$, and consequently

$$
d\in d\quad\Longleftrightarrow\quad d\notin d,
$$

which is impossible. Thus no such $A$ exists:

$$
\boxed{E\text{ is well-founded, without Choice or Foundation}.}
$$

This [power-set-predecessor relation](../../../../../../power-set-predecessor-relation.md) proof uses neither a descending sequence nor a comparison of possibly non-well-orderable [cardinalities](../../../../../../cardinality.md). It proves [well-foundedness](../../../../../../well-founded-relation.md) directly from the minimal-member definition.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
