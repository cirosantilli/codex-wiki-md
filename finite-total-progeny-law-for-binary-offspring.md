# Finite total progeny law for binary offspring

↑ **Parent:** [Total progeny of a branching process](total-progeny-of-a-branching-process.md)

For a [branching process](branching-process.md) starting from one individual with offspring two with probability $p$ and zero otherwise, the finite [total progeny](total-progeny-of-a-branching-process.md) is odd. Exploring individuals gives an active queue beginning at one, with increments $+1$ or $-1$. A first hit of zero at time $2j+1$ requires $j$ positive and $j+1$ negative increments and no earlier empty queue. The [Catalan number](catalan-number.md) $C_j=\binom{2j}j/(j+1)$ counts these admissible sequences, for example by the reflection principle after removing the final down step. Independence then gives the displayed mass formula.

If $p\ne1/2$, $b=4p(1-p)<1$ and $C_j\le4^j$, so $\mathbb P(K=2j+1)\le(1-p)b^j$. Choosing $c=\min\{-\log(1-p),-\tfrac12\log b\}>0$ bounds every finite mass by $e^{-c(2j+1)}$. This does not exclude an atom at infinity. In the supercritical case that atom has mass $(2p-1)/p$. At criticality $p=1/2$, the process dies out almost surely, but the [Catalan number](catalan-number.md) asymptotic gives masses proportional to $j^{-3/2}$ and hence infinite mean total progeny.

## ↑ Ancestors (6)

1. [Total progeny of a branching process](total-progeny-of-a-branching-process.md)
2. [Galton-Watson process](galton-watson-process-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
