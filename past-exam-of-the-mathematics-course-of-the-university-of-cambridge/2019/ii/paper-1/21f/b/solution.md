<h1 id="21f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $X=S^1\vee S^1$, the [wedge of two circles](../../../../../../wedge-of-two-circles.md), and label its oriented loops $a$ and $b$. For a fixed $n\geq3$, let

$$
\alpha=(1\ 2\ \cdots\ n),
\qquad
\beta=(1\ 2)
$$

be permutations of the fibre $\{1,\ldots,n\}$. Construct a labelled graph $\widehat X_n$ with these $n$ vertices, an oriented $a$-edge from $i$ to $\alpha(i)$, and an oriented $b$-edge from $i$ to $\beta(i)$. Map every vertex to the wedge point and each labelled edge homeomorphically onto its corresponding loop. Every vertex has exactly one incoming and one outgoing edge of each label, so this is an $n$-sheeted [permutation covering of a wedge of circles](../../../../../../permutation-covering-of-a-wedge-of-circles.md)

$$
p_n:\widehat X_n\longrightarrow X.
$$

It is connected because the $n$-cycle $\alpha$ acts transitively on the fibre.

A [deck transformation](../../../../../../deck-transformation.md) induces a permutation $\gamma$ of the vertices that commutes with both monodromy permutations $\alpha$ and $\beta$. Conversely, such a permutation determines a deck transformation, by the [deck transformation group as a monodromy centralizer](../../../../../../deck-transformation-group-as-a-monodromy-centralizer.md). The permutations $\alpha$ and $\beta$ generate $S_n$: the conjugates $\alpha^j\beta\alpha^{-j}$ include the adjacent transpositions, which generate the [symmetric group](../../../../../../symmetric-group.md). Hence $\gamma$ centralizes $S_n$ and lies in its [center of a group](../../../../../../center-of-a-group.md). For $n\geq3$, the center of $S_n$ is trivial, so $\gamma=1$. A deck transformation fixing one point is the identity by part (a), and therefore

$$
\boxed{\operatorname{Deck}(p_n)=\{1\}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21F](../../21f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
