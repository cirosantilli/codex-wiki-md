<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [probabilistic Banzhaf index](../../../../../probabilistic-banzhaf-index.md) satisfies **[cooperative-game symmetry](../../../../../symmetry-of-a-cooperative-game-value.md), the [null player](../../../../../null-player.md) axiom and [cooperative-game additivity](../../../../../additivity-of-a-cooperative-game-value.md), but not [cooperative-game efficiency](../../../../../efficiency-of-a-cooperative-game-value.md)**.

For [cooperative-game symmetry](../../../../../symmetry-of-a-cooperative-game-value.md), interchangeable players have $v(Ti)=v(Tj)$ for every $T$ omitting them. The [Banzhaf difference identity](../../../../../banzhaf-difference-identity.md) therefore gives equal indices. For a [null player](../../../../../null-player.md), every [marginal contribution](../../../../../marginal-contribution.md) in the defining average is zero, so its index is zero.

For [cooperative-game additivity](../../../../../additivity-of-a-cooperative-game-value.md), each [marginal contribution](../../../../../marginal-contribution.md) is additive:

$$
(v+w)(S\cup\{i\})-(v+w)(S)=[v(S\cup\{i\})-v(S)]+[w(S\cup\{i\})-w(S)].
$$

Averaging both sides over the same $2^{n-1}$ [coalitions](../../../../../coalition-game-theory.md) gives $\beta_i(v+w)=\beta_i(v)+\beta_i(w)$.

For failure of [cooperative-game efficiency](../../../../../efficiency-of-a-cooperative-game-value.md), the indices computed in part (b) sum to $5/4$, whereas the grand-[coalition](../../../../../coalition-game-theory.md) value is one. This is already a counterexample. Independently, a three-player majority game gives each player index $1/2$, also exceeding the total value when summed. Pivotality averaged over independently chosen [coalitions](../../../../../coalition-game-theory.md) does not telescope in the way the ordering-average [Shapley value](../../../../../shapley-value.md) does.

## ↑ Ancestors (11)

1. [D](../d.md)
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
