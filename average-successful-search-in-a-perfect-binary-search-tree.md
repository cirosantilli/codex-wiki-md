# Average successful search in a perfect binary search tree

↑ **Parent:** [Binary search](binary-search.md)

For $n=2^k-1$ distinct keys and a uniformly chosen present target, early-return [binary search](binary-search.md) takes mean $k-1+k/n$ iterations. There are $2^d$ targets needing $d+1$ probes, so sum $(d+1)2^d$ over depths zero through $k-1$ and divide by $n$. A boundary search that always closes the interval takes exactly $k$ iterations. Their expected difference is $1-k/n<1$, even though an individual shallow target can save many probes.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
