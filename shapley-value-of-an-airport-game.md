# Shapley value of an airport game

↑ **Parent:** [Airport problem](airport-problem.md)

Suppose the distinct required runway lengths are $0=s_0<s_1<\cdots<s_k$, with $n_i>0$ users of type $i$, constant cost $\lambda\geq0$ per unit length, and suffix counts $N_i=\sum_{\ell=i}^k n_\ell$. Then every type-$j$ user has the displayed [Shapley value](shapley-value.md). For layer $i$, exactly $N_i$ users require it. The first of them in a uniformly random [permutation](permutation.md) contributes its entire cost $\lambda(s_i-s_{i-1})$. Each requiring user has [probability](probability.md) $1/N_i$ of being first. [Linearity of the Shapley value](linearity-of-the-shapley-value.md) sums these expected [marginal contributions](marginal-contribution.md) across the layers that user needs.

The allocation lies in the cost [core](core-game-theory.md). Its payments sum to the full runway cost. For any [coalition](coalition-game-theory.md) $S$, its total payment toward layer $i$ is $\lambda(s_i-s_{i-1})|S\cap R_i|/N_i$, where $R_i$ is the set of users requiring that layer. This is zero if $S$ needs no such layer, and at most the full layer cost otherwise. Summing gives $\sum_{j\in S}\phi_j\leq c(S)$. Suffix counts followed by prefix sums compute all distinct type payments in $O(k)$ arithmetic operations.

## ↑ Ancestors (9)

1. [Airport problem](airport-problem.md)
2. [Cooperative cost game](cooperative-cost-game.md)
3. [Transferable utility game](transferable-utility-game.md)
4. [Cooperative game theory](cooperative-game-theory.md)
5. [Game theory](game-theory-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Airport problem](airport-problem.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/computational-game-theory/3/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/computational-game-theory/3/f/solution.md)
