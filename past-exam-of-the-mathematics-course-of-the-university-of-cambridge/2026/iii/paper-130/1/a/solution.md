<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Canonical Ramsey theorem](../../../../../../canonical-ramsey-theorem.md) says that for every map $c:[\mathbb N]^{(r)}\to C$, with no restriction on the colour set $C$, there are an infinite set $X=\{x_1<x_2<\cdots\}$ and $I\subseteq\{1,\ldots,r\}$ such that, for increasing tuples from $X$,

$$
c(\{u_1,\ldots,u_r\})=c(\{v_1,\ldots,v_r\})
\quad\Longleftrightarrow\quad
u_i=v_i\text{ for every }i\in I.
$$

To prove it, define an equivalence relation on $[\mathbb N]^{(r)}$ by equality of colours. Two ordered pairs of $r$-sets have one of finitely many intersection-order types. Successively apply the infinite [Ramsey theorem](../../../../../../ramsey-theorem.md) to obtain an infinite $X$ on which, for each type, equivalence has a constant truth value. Let $I$ consist of those coordinates whose replacement, with all other coordinates fixed and order preserved, changes the equivalence class. Homogeneity of the pair types shows first that this does not depend on the chosen tuple. Changing coordinates one at a time then shows that agreement on $I$ implies equivalence; reversing the same chain shows that disagreement at a coordinate in $I$ implies inequivalence. This gives the displayed canonical form.

For $r=2$, the four choices of $I$ give exactly the constant, minimum, maximum, and injective colourings. Suppose the asserted finite result failed for some $s$. For every $n$ choose an equivalence relation on $[n]^{(2)}$ having no canonical $s$-set. These finite bad relations form a finitely branching tree under restriction. [König infinity lemma](../../../../../../konig-s-lemma.md) gives an infinite branch, hence a colouring-equivalence relation on $[\mathbb N]^{(2)}$ with no canonical $s$-set. The canonical theorem supplies an infinite canonical set, whose first $s$ vertices give a contradiction. Therefore a suitable finite $n$ exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
