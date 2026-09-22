# Lattice-path interpretation of Gaussian binomial coefficients

↑ **Parent:** [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)

Use [lattice paths](lattice-path.md) with $k$ north steps and $n-k$ east steps, beginning at $(0,0)$. Let $A(P)$ be the [sum](sum.md) of the horizontal coordinates of its north steps, equivalently the number of unit cells to their left inside the $k$-by-$(n-k)$ [rectangle](rectangle.md). A north step in zero-based word position $j_i$ has $i-1$ earlier north steps, so its horizontal coordinate is $j_i-(i-1)$. The [Gaussian binomial coefficient recurrence](gaussian-binomial-coefficient-recurrence.md) therefore counts these [lattice paths](lattice-path.md) with weight $t^{A(P)}$.

For $n=4,k=2$, the words `NNEE`, `NENE`, `NEEN`, `ENNE`, `ENEN`, `EENN` have respective [areas](surface-area.md) $0,1,2,2,3,4$. The word `NEEN` contributes $t^2$ because the two north steps occur at horizontal coordinates zero and two. These paths never move south or west; allowing such extra steps would change the collection being counted.

## ↑ Ancestors (6)

1. [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)
2. [Binomial coefficient](binomial-coefficient.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)
- [Partition interpretation of Gaussian binomial coefficients](partition-interpretation-of-gaussian-binomial-coefficients.md)
