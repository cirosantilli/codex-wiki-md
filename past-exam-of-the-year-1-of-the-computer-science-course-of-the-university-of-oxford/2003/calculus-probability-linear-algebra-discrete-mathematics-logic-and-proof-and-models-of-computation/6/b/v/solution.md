<h1 id="6/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The answer is **no**, even when both original [binary relations](../../../../../../binary-relation.md) are [equivalence relations](../../../../../../equivalence-relation.md). On $X=\{a,b,c\}$, let $R_1$ have [equivalence classes](../../../../../../equivalence-class.md) $\{a,b\},\{c\}$ and $R_2$ have [equivalence classes](../../../../../../equivalence-class.md) $\{a\},\{b,c\}$. Each is a [transitive relation](../../../../../../transitive-relation.md) and, by the earlier proof, a [Euclidean relation](../../../../../../euclidean-relation.md).

Use exactly the paper's convention for [composition of relations](../../../../../../composition-of-relations.md): $xRy$ means $xR_1z$ and $zR_2y$ for some $z$. The possible successors are

$$
R(a)=R(b)=\{a,b,c\},\qquad R(c)=\{b,c\}.
$$

Indeed, from $a$ or $b$ the first step can reach $a$ or $b$, whose $R_2$ successors together exhaust $X$; from $c$ the first step must stay at $c$, whose $R_2$ successors are only $b,c$. Consequently $cRb$ and $bRa$, but not $cRa$. Therefore

$$
\boxed{R_1\text{ and }R_2\text{ transitive and Euclidean does not force }R\text{ transitive}.}
$$

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
