<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [simple cooperative game](../../../../../../simple-cooperative-game.md), the [Shapley value](../../../../../../shapley-value.md) is the [probability](../../../../../../probability.md) that a player is pivotal in a uniformly random ordering. Symmetry gives one value for permanent members and another for nonpermanent members.

A particular nonpermanent member is pivotal exactly when all five permanent members and exactly three of the other nine nonpermanent members precede them. The predecessor set then has size eight. There are $\binom93$ such sets, each giving $8!6!$ orderings. Their [Shapley value](../../../../../../shapley-value.md) is therefore

$$
\beta=\binom93\frac{8!6!}{15!}=\frac4{2145}.
$$

Every ordering has exactly one pivotal member, since the empty [coalition](../../../../../../coalition-game-theory.md) loses and the full [coalition](../../../../../../coalition-game-theory.md) wins. This proves efficiency directly: $5\alpha+10\beta=1$, where $\alpha$ is the value of each permanent member. Hence

$$
\boxed{\alpha=\frac{421}{2145},\qquad\beta=\frac4{2145}.}
$$

The vector has five entries $421/2145$ and ten entries $4/2145$. As a check, a permanent member is pivotal when they are last among the permanent members and occupy a position from nine to fifteen; counting those orderings gives the same $\alpha$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
