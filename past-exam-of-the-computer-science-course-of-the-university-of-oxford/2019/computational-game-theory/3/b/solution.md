<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the inclusive quota: a [coalition](../../../../../coalition-game-theory.md) wins at weight **at least $25$**. For each player, count losing predecessor [coalitions](../../../../../coalition-game-theory.md) that become winning when that player joins. Group these swing counts by predecessor [cardinality](../../../../../cardinality.md) $t=0,1,2,3$:

| Player and weight | Swing counts $(n_{i,0},n_{i,1},n_{i,2},n_{i,3})$ | [Shapley value](../../../../../shapley-value.md) | [Banzhaf index](../../../../../probabilistic-banzhaf-index.md) |
| --- | --- | --- | --- |
| $1:\ 15$ | $(0,1,3,1)$ | $7/12$ | $5/8$ |
| $2:\ 10$ | $(0,1,2,0)$ | $1/4$ | $3/8$ |
| $3:\ 5$ | $(0,0,1,0)$ | $1/12$ | $1/8$ |
| $4:\ 5$ | $(0,0,1,0)$ | $1/12$ | $1/8$ |

For example, player one is pivotal for predecessor [coalitions](../../../../../coalition-game-theory.md) $\{2\}$, $\{2,3\}$, $\{2,4\}$, $\{3,4\}$ and $\{2,3,4\}$. Player three is pivotal only for $\{1,4\}$; player four has the symmetric counterpart.

Each swing contributes $1/8$ to the [probabilistic Banzhaf index](../../../../../probabilistic-banzhaf-index.md). For the [Shapley value](../../../../../shapley-value.md), a swing with $t$ predecessors contributes $t!(3-t)!/4!$, which is $1/4,1/12,1/12,1/4$ for the four possible sizes. Applying these weights to the table gives

$$
\boxed{\phi=(7/12,\,1/4,\,1/12,\,1/12),\qquad\beta=(5/8,\,3/8,\,1/8,\,1/8).}
$$

The [Shapley values](../../../../../shapley-value.md) sum to one. The unnormalized [Banzhaf indices](../../../../../probabilistic-banzhaf-index.md) sum to $5/4$; they must not be replaced by normalized shares in this part.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
