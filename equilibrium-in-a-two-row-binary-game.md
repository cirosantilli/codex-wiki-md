# Equilibrium in a two-row binary game

↑ **Parent:** [Binary game](binary-game.md)

Write column $j$ of a two-row [binary game](binary-game.md) as $((a_j,c_j),(b_j,d_j))^T$, with the row player's [payoff](payoff.md) first. If there is no pure [Nash equilibrium](nash-equilibrium.md), the column player's maximum [payoff](payoff.md) in each row must be one. Otherwise every column would be a [best response](best-response.md) in a zero-payoff row, and excluding an equilibrium there would force the opposite row to dominate in every column, giving an equilibrium in that opposite row.

A column maximizing the column player's top-row [payoff](payoff.md) must then have $(a_j,b_j)=(0,1)$, or its top cell would be an equilibrium. Its bottom column-player [payoff](payoff.md) must be zero, or its bottom cell would be one. Thus a column $((0,1),(1,0))^T$ occurs. The same argument for the bottom row produces $((1,0),(0,1))^T$. No column can give the column player [payoffs](payoff.md) $(1,1)$, since a row-player [best response](best-response.md) within that column would be a pure equilibrium.

Consequently, if neither pure equilibrium is found, mix equally over the two rows and equally over those two special columns. The row player's two [expected payoffs](expected-payoff.md) are $1/2$; every column gives the column player at most $1/2$, and the supported columns achieve $1/2$. This is a [Nash equilibrium](nash-equilibrium.md). Computing the two row maxima, scanning for pure equilibria and locating the two special columns takes $O(n)$ [running time](running-time.md) for $n$ columns.

## ↑ Ancestors (7)

1. [Binary game](binary-game.md)
2. [Normal-form game](normal-form-game.md)
3. [Game theory](game-theory-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/computational-game-theory/2/f/solution.md)
