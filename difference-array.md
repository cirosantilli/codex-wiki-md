# Difference array

↑ **Parent:** [Array (data structure)](array-data-structure.md)

For an array $a$, its difference array stores $d_0=a_0$ and $d_i=a_i-a_{i-1}$ for $i>0$. The original entries are [prefix sums](prefix-sum.md) of $d$. Adding $v$ on indices $[l,r]$ requires only $d_l\mathrel{+}=v$ and, when present, $d_{r+1}\mathrel{-}=v$.

## ↑ Ancestors (4)

1. [Array (data structure)](array-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
