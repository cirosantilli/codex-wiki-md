# Chain lower bound for a submodular set function

↑ **Parent:** [Submodular set function](submodular-set-function.md)

Let $f$ be a [normalised set function](normalised-set-function.md) that is a [submodular set function](submodular-set-function.md), and order a finite [subset](subset.md) $T=\{x_1,\ldots,x_n\}$. Set $P_j=\{x_1,\ldots,x_j\}$ and $P_0=\varnothing$. Then the displayed inequality holds for every $U\subseteq T$, with equality for $U=T$. The right side is a [modular set function](modular-set-function.md) lying below $f$ on the [power set](power-set.md) of $T$ and touching it at the top.

**Proof.** Reveal the elements of $U$ in the chosen order. Immediately before adding $x_j\in U$, the conditioning [set](set-split.md) is $U\cap P_{j-1}\subseteq P_{j-1}$. By [diminishing returns](diminishing-returns-characterization-of-submodularity.md), its [marginal increment](marginal-increment-of-a-set-function.md) is at least $f(P_j)-f(P_{j-1})$. Sum and use $f(\varnothing)=0$. The same [telescoping sum](telescoping-sum.md) gives equality at $T$. The individual increments need not be nonnegative.

## ↑ Ancestors (8)

1. [Submodular set function](submodular-set-function.md)
2. [Set function](set-function.md)
3. [Function](function-split.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Exact-cover inequality for submodular set functions](exact-cover-inequality-for-submodular-set-functions.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/1/e/solution.md)
