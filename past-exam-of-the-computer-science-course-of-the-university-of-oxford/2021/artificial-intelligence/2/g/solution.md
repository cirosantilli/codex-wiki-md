<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

**Choose one global direction and impose it on every adjacent pair.** Keep $X_i\in\{1,\ldots,m\}$, introduce $D\in\{+,-\}$, and impose for each $i<n$ the relation

$$
R(D,X_i,X_{i+1})\iff
(D=+\land X_i<X_{i+1})\lor(D=-\land X_i>X_{i+1}).
$$

Because the same $D$ occurs everywhere, [transitivity](../../../../../transitive-relation.md) gives either a strictly increasing whole sequence or a strictly decreasing one. Choosing independently between $<$ and $>$ at each [edge](../../../../../edge-of-a-graph.md) would merely require adjacent values to differ and would incorrectly allow zigzags.

If a binary formulation is required, replace each ternary relation by a [hidden-variable encoding](../../../../../hidden-variable-encoding.md). Add a [variable](../../../../../variable-mathematics.md) $Y_i$ with domain

$$
\{(+,a,b):1\le a<b\le m\}\cup\{(-,a,b):1\le b<a\le m\}.
$$

Use three [binary constraints](../../../../../binary-constraint.md): the sign component of $Y_i$ equals $D$, its first numeric component equals $X_i$, and its second equals $X_{i+1}$. These enforce exactly the relation above while leaving the original [variable](../../../../../variable-mathematics.md) domains unchanged. Each auxiliary domain has $m(m-1)$ values.

For $n\ge2$, the projected solutions in the original $X_i$ [variables](../../../../../variable-mathematics.md) number $2\binom mn$ when $m\ge n$, and zero otherwise. In particular $m=n=3$ gives exactly $(1,2,3)$ and $(3,2,1)$. For $n=1$, direction is irrelevant and the projected solutions number $m$, not $2m$.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
