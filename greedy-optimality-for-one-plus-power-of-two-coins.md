# Greedy optimality for one-plus-power-of-two coins

↑ **Parent:** [Coin change problem](coin-change-problem.md)

For denominations $1$ and $c_j=2^j+1$ with $0\leq j\leq k$, greedy minimizes coin count. Among optimal representations choose a lexicographically maximal descending denomination-count vector. Two unit coins can be replaced by one two; two $c_j$ below the largest can be replaced by $c_{j+1}+1$ without increasing count but improving that vector. Thus all smaller denominations occur at most once. For the coins below $c_j$, write their value as $L=B+r$, where $r$ is their count and $B\leq2^j-1$ is the sum of their distinct power-of-two parts. If $L\geq c_j$, one $c_j$ and $L-c_j$ units use $L-2^j\leq r-1$ coins, contradicting optimality. Therefore the residual below each denomination is smaller than it, forcing precisely the greedy quotients.

## ↑ Ancestors (6)

1. [Coin change problem](coin-change-problem.md)
2. [Dynamic programming](dynamic-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
