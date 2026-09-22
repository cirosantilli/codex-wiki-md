<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Rado graph](../../../../../rado-graph.md) on the [natural numbers](../../../../../natural-number.md). Interpret the binary relation by

$$
\boxed{E(i,j)\quad\Longleftrightarrow\quad
[i<j\land\mathit{Bit}(i,j)]\lor[j<i\land\mathit{Bit}(j,i)].}
$$

The relation is symmetric by its definition, and $E(i,i)$ is always false. Thus this [first-order structure](../../../../../first-order-structure.md) satisfies $F_1$ and $F_2$.

To verify an extension axiom, take distinct $x_1,\ldots,x_n$. Choose a [natural number](../../../../../natural-number.md) $k$ larger than every $x_i$ and put

$$
y=2^k+\sum_{i=1}^{m-1}2^{x_i}.
$$

The powers are distinct, so there are no carries in this [binary representation](../../../../../binary-number.md). In particular $y>x_i$ for every $i$, and the [bit](../../../../../bit.md) in position $x_i$ is one exactly when $i<m$. Therefore $y$ is different from all the given [vertices](../../../../../vertex-graph-theory.md), is adjacent to $x_1,\ldots,x_{m-1}$, and is not adjacent to the others. If the $x_i$ are not distinct, the antecedent of the extension axiom is false, so it places no restriction. The case $n=0$, if included in the convention for [natural numbers](../../../../../natural-number.md), simply asks for a nonempty domain, which this [first-order structure](../../../../../first-order-structure.md) has.

For example, prescribing adjacency to $1$ and $3$ and nonadjacency to $2$ permits $k=4$ and $y=16+2+8=26$, whose [binary representation](../../../../../binary-number.md) is $11010$. This explicitly realizes the required pattern. Hence

$$
\boxed{(\mathbb N,E)\models T_0.}
$$

Reordering a tuple makes the extension axioms applicable to any two disjoint finite sets of [vertices](../../../../../vertex-graph-theory.md), with any desired adjacency and nonadjacency pattern. This is the extension property defining the [theory of the random graph](../../../../../theory-of-the-random-graph.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
