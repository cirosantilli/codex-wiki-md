# Minimax theorem

↑ **Parent:** [Zero-sum game](zero-sum-game.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimax_theorem)

For every real $m\times n$ [payoff matrix](payoff-matrix.md) $A$ of a two-player [zero-sum game](zero-sum-game.md), the [minimax theorem](minimax-theorem.md) states

$$
\max_{x\in\Delta_m}\min_{y\in\Delta_n}x^{\mathsf T}Ay
=\min_{y\in\Delta_n}\max_{x\in\Delta_m}x^{\mathsf T}Ay=v,
$$

where $\Delta_m,\Delta_n$ are the players' [probability simplices](probability-simplex.md). Both outer optima are attained. The row player's [security level payoff](security-level-payoff.md) is the largest [payoff](payoff.md) it can guarantee against all opposing choices; the column player can hold that [payoff](payoff.md) to the same number $v$, the [value of a zero-sum game](value-of-a-zero-sum-game.md). For optimal $x^*,y^*$,

$$
x^{\mathsf T}Ay^*\leq v=(x^*)^{\mathsf T}Ay^*\leq(x^*)^{\mathsf T}Ay
\quad\text{for all }x\in\Delta_m,\ y\in\Delta_n.
$$

These are exactly the [Nash equilibrium](nash-equilibrium.md) inequalities under the row-maximizes, column-minimizes convention. Conversely, a [Nash equilibrium](nash-equilibrium.md) of this two-player [zero-sum game](zero-sum-game.md) supplies both guarantees. This equality explains why independent worst-case [optimization](mathematical-optimization-split.md) solves the opposing incentives in this special class.

Allowing [mixed strategies](mixed-strategy.md) is essential. For [matching pennies](matching-pennies.md), $A=\left(\begin{smallmatrix}1&-1\\-1&1\end{smallmatrix}\right)$. Restricting both players to [pure strategies](pure-strategy.md) gives $\max_i\min_j A_{ij}=-1$ and $\min_j\max_i A_{ij}=1$. Allowing [mixed strategies](mixed-strategy.md) closes the gap: each fair mixture guarantees zero, so $v=0$. These guarantees hold even if the opponent knows the mixture's [probabilities](probability.md), provided the opponent does not observe the sampled choice before choosing.

John von Neumann proved the two-player [zero-sum game](zero-sum-game.md) result in [Zur Theorie der Gesellschaftsspiele, Mathematische Annalen 100, 295–320 (1928)](https://link.springer.com/article/10.1007/BF01448847); the original article's footnote 7 explicitly discusses the equality of max–min and min–max. Nash's [1950 paper](https://pmc.ncbi.nlm.nih.gov/articles/PMC1063129/) states that existence of a [Nash equilibrium](nash-equilibrium.md) is equivalent to this result in the two-player [zero-sum game](zero-sum-game.md) case, and extends existence to all [finite games](finite-game.md).

## ↑ Ancestors (6)

1. [Zero-sum game](zero-sum-game.md)
2. [Game theory](game-theory-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Minimax theorem](minimax-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/21h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/21h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/18h/solution.md)
- [Value of a zero-sum game](value-of-a-zero-sum-game.md)
- [Zero-sum game](zero-sum-game.md)
