<h1 id="16h/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Introduce a propositional variable $P_{x,i}$ for every $x\in X$ and $i\in\{1,\ldots,100\}$. Form a theory containing, for every $x$, clauses saying that exactly one of

$$
P_{x,1},\ldots,P_{x,100}
$$

is true, and, for every $y\in L_x$ and every $i$, the clause

$$
\neg(P_{x,i}\land P_{y,i}).
$$

Every finite subset of these clauses mentions only finitely many elements, forming a finite set $Y\subset X$. The assumed coloring $f_Y$ gives that finite subset a model. The [propositional compactness theorem](../../../../../../../propositional-compactness-theorem.md), equivalently the propositional consequence of first-order [compactness](../../../../../../../compactness-theorem.md), therefore gives a model of all the clauses.

For each $x$, let $F(x)$ be the unique $i$ for which $P_{x,i}$ is true. The edge clauses ensure that $F(x)\ne F(y)$ whenever $y\in L_x$. Hence

$$
\boxed{F:X\longrightarrow\{1,\ldots,100\}}
$$

has the required property.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [16H](../../../16h.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
