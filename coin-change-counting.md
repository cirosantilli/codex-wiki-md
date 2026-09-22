# Coin-change counting

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

Count [multisets](multiset.md) of allowed positive coin values whose [sum](sum.md) is a target. Initialize $w(0)=1$ and $w(s)=0$ for $s>0$. For each coin $c$, update $w(s)\leftarrow w(s)+w(s-c)$ in increasing order of $s\ge c$. The outer loop over coins counts each [multiset](multiset.md) once while allowing repeated use of a coin.

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
