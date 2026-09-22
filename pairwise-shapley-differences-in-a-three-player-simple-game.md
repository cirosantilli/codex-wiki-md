# Pairwise Shapley differences in a three-player simple game

↑ **Parent:** [Shapley value](shapley-value.md)

For three distinct players $i,j,k$ in a normalized [simple cooperative game](simple-cooperative-game.md), enumerate the predecessor [coalitions](coalition-game-theory.md) in the [Shapley value](shapley-value.md) formula:

$$
\phi_i=\tfrac13v(\{i\})+\tfrac16\bigl(v(\{i,j\})-v(\{j\})\bigr)+\tfrac16\bigl(v(\{i,k\})-v(\{k\})\bigr)+\tfrac13\bigl(1-v(\{j,k\})\bigr).
$$

Subtracting the formula with $i$ and $j$ exchanged proves the displayed identity. Every [coalition](coalition-game-theory.md) value is zero or one, so $2(\phi_i-\phi_j)$ is an [integer](integer-split.md). This rules out, for example, coordinates differing by $1/6$, although each may separately satisfy the [Shapley value denominator in a simple game](shapley-value-denominator-in-a-simple-game.md). The difference identity itself holds for arbitrary three-player [transferable utility games](transferable-utility-game.md); the integer restriction uses the zero-one values.

## ↑ Ancestors (8)

1. [Shapley value](shapley-value.md)
2. [Transferable utility game](transferable-utility-game.md)
3. [Cooperative game theory](cooperative-game-theory.md)
4. [Game theory](game-theory-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2022/computational-game-theory/4/c/iv/solution.md)
