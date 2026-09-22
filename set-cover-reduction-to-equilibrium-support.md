# Set cover reduction to equilibrium support

↑ **Parent:** [Set cover problem](set-cover-problem.md)

Assume $2\leq k<m$ and $\bigcup_iS_i=S$. Construct a two-player game with row $i$ for $S_i$ and columns $0,1,\ldots,n$. Column $0$ pays both players one; column $j>0$ pays $(1,0)$ when $j\in S_i$, and $(0,k/(k-1))$ otherwise. There is a [Nash equilibrium](nash-equilibrium.md) whose row player's [support of a mixed strategy](support-of-a-mixed-strategy.md) has size $k$ exactly when $k$ rows cover the universe. A uniform mixture on a cover makes column $0$ a [best response](best-response.md). Conversely, if some element is uncovered by the support, the column player's [best responses](best-response.md) are uncovered elements and the row player's current payoff is zero. The union promise provides a profitable row deviation. Without the union promise the equivalence is false: a globally uncovered element is a [best response](best-response.md) against every row mixture.

// Target: mathematical-optimization.bigb

## ↑ Ancestors (9)

1. [Set cover problem](set-cover-problem.md)
2. [NP-completeness](np-completeness.md)
3. [NP-hardness](np-hardness.md)
4. [Polynomial-time many-one reduction](polynomial-time-many-one-reduction.md)
5. [Polynomial-time reduction](polynomial-time-reduction.md)
6. [Computational complexity theory](computational-complexity-theory.md)
7. [Theoretical computer science](theoretical-computer-science.md)
8. [Computer science](computer-science-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-38/3/solution.md)
