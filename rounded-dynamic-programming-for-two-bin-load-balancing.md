# Rounded dynamic programming for two-bin load balancing

↑ **Parent:** [Two-bin load balancing](two-bin-load-balancing.md)

For integer weights, subset-sum [dynamic programming](dynamic-programming.md) finds the greatest achievable total at most $s/2$ in time $O(ns)$, where $s$ is the total weight. For rational weights and $0<\varepsilon<1$, scale by $K=\varepsilon s/(2n)$ and round down to $q_i=\lfloor w_i/K\rfloor$. The scaled total is at most $2n/\varepsilon$, so exact dynamic programming costs $O(n^2/\varepsilon)$ arithmetic operations. Lifting its partition to the original weights increases the maximum load by at most $nK\leq\varepsilon\operatorname{OPT}$. Thus it is a [fully polynomial-time approximation scheme](fully-polynomial-time-approximation-scheme.md) for this two-bin problem. Bit complexity also accounts for the rational input and epsilon encodings.

## ↑ Ancestors (6)

1. [Two-bin load balancing](two-bin-load-balancing.md)
2. [Integer programming](integer-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-40/6/c/solution.md)
