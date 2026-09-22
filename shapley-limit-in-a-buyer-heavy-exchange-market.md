# Shapley limit in a buyer-heavy exchange market

↑ **Parent:** [Shapley value](shapley-value.md)

For $k$ unit sellers and $3k$ unit buyers with unit surplus per trade, a coalition's value is the smaller of its seller and buyer counts. Give each player an independent uniform arrival time. Conditional on a specified seller arriving at time $t$, the previous buyers and other sellers have independent binomial counts $B\sim\operatorname{Bin}(3k,t)$ and $S\sim\operatorname{Bin}(k-1,t)$. The seller contributes one exactly when $B>S$. For fixed positive $t$ this probability tends to one; a Chebyshev bound and a split near $t=0$ also give an explicit uniform integral estimate. Averaging gives seller [Shapley value](shapley-value.md) tending to one. Efficiency and role symmetry give $s_k+3b_k=1$, hence the buyer value tends to zero.

## ↑ Ancestors (8)

1. [Shapley value](shapley-value.md)
2. [Transferable utility game](transferable-utility-game.md)
3. [Cooperative game theory](cooperative-game-theory.md)
4. [Game theory](game-theory-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-34/4/solution.md)
