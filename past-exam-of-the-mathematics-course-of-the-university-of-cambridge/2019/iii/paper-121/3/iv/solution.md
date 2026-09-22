<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Fix names $\dot x,\dot a_1,\ldots,\dot a_n\in M$ and a [first-order formula](../../../../../../first-order-formula.md) $\varphi$. Using the [syntactic forcing relation](../../../../../../syntactic-forcing-relation.md), form in $M$ the name

$$
\dot y=\{(\tau,r):\exists q\,((\tau,q)\in\dot x\land r\leq q\land r\Vdash^*\varphi(\tau,\dot a_1,\ldots,\dot a_n))\}.
$$

This is a set by the [axiom schema of separation](../../../../../../axiom-schema-of-specification.md) in $M$. If $(\tau,r)\in\dot y$ and $r\in G$, then the [forcing theorem](../../../../../../forcing-theorem.md) gives both $\tau^G\in\dot x^G$ and $\varphi(\tau^G,\dot a_1^G,\ldots,\dot a_n^G)$. Conversely, if $z\in\dot x^G$ satisfies $\varphi$, choose $(\tau,q)\in\dot x$ with $q\in G$ and $\tau^G=z$. The truth direction of the forcing theorem supplies $s\in G$ forcing $\varphi(\tau,\dot a_1,\ldots,\dot a_n)$; directedness of $G$ gives $r\in G$ below both $q$ and $s$, so $(\tau,r)\in\dot y$.

Thus

$$
\dot y^G=\{z\in\dot x^G:M[G]\models\varphi(z,\dot a_1^G,\ldots,\dot a_n^G)\}.
$$

Every instance has such a witness, so [separation in a generic extension](../../../../../../separation-in-a-generic-extension.md) proves **$M[G]\models$ Separation.**

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
