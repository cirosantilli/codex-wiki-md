<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Several other approaches illustrate the range between fast heuristics, certified bounds and approximation schemes.

Sorting weights in decreasing order before greedy assignment avoids the example $1,1,2$: it starts with the weight $2$, then places both unit weights in the other bin, giving the optimum. This is a useful scheduling heuristic, although improvement on one example is not a proof of an arbitrary claimed [approximation ratio](../../../../../../approximation-ratio.md). Local improvement can additionally move a single item or swap items between bins whenever it reduces the maximum load; it produces a local optimum, which need not be global.

A linear-programming relaxation replaces $z_i\in\{0,1\}$ by $0\leq z_i\leq1$. The choice $z_i=1/2$ for every item gives load $s/2$ in both bins, and summing the load constraints shows that no smaller relaxed value is possible. Together with the indivisibility bound $w_{\max}$ this provides a lower bound $L=\max(s/2,w_{\max})$ on the integer optimum. Any feasible heuristic schedule gives an upper bound $U$. Their ratio $U/L$ is a computable quality certificate. Branch-and-bound can improve these bounds by fixing assignment variables and solving subproblems, although worst-case exact running time need not be polynomial.

For integer weights one can instead solve the problem exactly by [dynamic programming](../../../../../../dynamic-programming.md). Start with attainable subset sums $T_0=\{0\}$ and update

$$
T_j=T_{j-1}\cup\{t+w_j:t\in T_{j-1}\},
$$

discarding values above $\lfloor s/2\rfloor$. Let $q$ be the largest retained sum. Choosing that subset for one bin gives loads $q,s-q$ and maximum $s-q$, which is optimal because every partition has a lighter side of weight at most $s/2$. The running time $O(ns)$ is pseudopolynomial: it depends on numeric magnitude, not merely the binary length of $s$.

This exact algorithm also yields [rounded dynamic programming for two-bin load balancing](../../../../../../rounded-dynamic-programming-for-two-bin-load-balancing.md). For rational weights and $0<\varepsilon<1$, choose $K=\varepsilon s/(2n)$ and scaled integer weights $q_i=\lfloor w_i/K\rfloor$. Their total is at most $2n/\varepsilon$, so exact [dynamic programming](../../../../../../dynamic-programming.md) on them costs $O(n^2/\varepsilon)$ arithmetic operations. Let $Y'$ be its optimal scaled maximum load. The original optimal partition is feasible for the scaled problem with load at most $Y^*/K$, so $KY'\leq Y^*$. When the scaled partition is lifted, each bin contains at most $n$ rounding errors, each smaller than $K$. Therefore its original maximum load satisfies

$$
Y\leq KY'+nK\leq Y^*+\frac{\varepsilon s}{2}\leq(1+\varepsilon)Y^*.
$$

This is a [fully polynomial-time approximation scheme](../../../../../../fully-polynomial-time-approximation-scheme.md): for each requested tolerance it gives a certified feasible solution in time polynomial in the encoded rational input and $1/\varepsilon$, with rational arithmetic accounted for. It works here because two-bin balancing has the subset-sum structure; one cannot infer that arbitrary combinatorial optimization problems admit such a scheme.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
