# Discrete location game

↑ **Parent:** [Normal-form game](normal-form-game.md)

A [discrete location game](discrete-location-game.md) can model firms choosing sites from $\{1,\ldots,k\}$ while customers at those sites choose a nearest firm. The customer masses, distance rule, permission to share a location and rule for ties are part of the model. For two firms, customer value two per site and equal splitting of ties, the [payoff](payoff.md) to a firm at $x$ against one at $y$ is

$$
u(x,y)=\begin{cases}x+y-1,&x<y,\\k,&x=y,\\2k-x-y+1,&x>y.\end{cases}
$$

For $x<y$, counting sites strictly left of the midpoint and assigning half of an equidistant site's value gives $x+y-1$, whether $x+y$ is [even](even-function.md) or [odd](odd-function.md). The other firm receives the remainder, so this is a [constant-sum game](constant-sum-game.md) with total $2k$. Changing tie priority can fundamentally change its [Nash equilibria](nash-equilibrium.md), especially when co-location is permitted.

**Table of contents**

- [Final entrant payoff in a discrete location game](final-entrant-payoff-in-a-discrete-location-game.md)

## ↑ Ancestors (6)

1. [Normal-form game](normal-form-game.md)
2. [Game theory](game-theory-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Discrete location game](discrete-location-game.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/computational-game-theory/1/a/solution.md)
