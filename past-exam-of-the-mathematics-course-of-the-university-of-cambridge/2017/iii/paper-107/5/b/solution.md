<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work first with essential bounds. On a [Euclidean ball](../../../../../../euclidean-ball.md) $B_R(x_0)\Subset B_1$, put $M=\operatorname*{ess\,sup}_{B_R}u$, $m=\operatorname*{ess\,inf}_{B_R}u$ and $\omega=M-m$. The functions $M-u$ and $u-m$ are nonnegative [weak solutions](../../../../../../weak-solution.md), hence [weak supersolutions](../../../../../../weak-supersolution-of-a-divergence-form-elliptic-equation.md). In $B_{R/2}$, at least one of the sets $\{u\leq(M+m)/2\}$ and $\{u\geq(M+m)/2\}$ has at least half the measure.

In the first case, the [Weak Harnack inequality](../../../../../../weak-harnack-inequality.md) applied to $M-u$ gives

$$
C_H\bigl(M-\operatorname*{ess\,sup}_{B_{R/2}}u\bigr)
\geq\left(\frac1{|B_{R/2}|}\int_{B_{R/2}}(M-u)^q\right)^{1/q}
\geq2^{-1-1/q}\omega.
$$

In the second case, applying it to $u-m$ gives the same lower bound for the improvement of the minimum. Thus the [oscillation decay estimate](../../../../../../oscillation-decay-estimate.md) is

$$
\boxed{\operatorname{osc}_{B_{R/2}}u\leq\tau\operatorname{osc}_{B_R}u,
\qquad \tau=1-C_H^{-1}2^{-1-1/q}\in(0,1).}
$$

This measure argument works even when $q<1$, avoiding a false use of the triangle inequality in that range.

Iteration yields $\operatorname{osc}_{B_r(x_0)}u\leq C(r/R)^\mu\operatorname{osc}_{B_R(x_0)}u$, with, for example, $\mu=\min\{1/2,-\log\tau/\log2\}\in(0,1)$. At [Lebesgue points](../../../../../../lebesgue-point.md) the shrinking oscillations define a unique continuous representative, and the estimate extends to every point by continuity. For $x,y\in B_{1/4}$ at distance less than $1/4$, apply the estimate to a [Euclidean ball](../../../../../../euclidean-ball.md) centred at $x$ with initial radius $1/2$ and final radius comparable to $|x-y|$. This [Euclidean ball](../../../../../../euclidean-ball.md) stays in $B_1$. Larger distances use the trivial bound $2\|u\|_\infty$. We obtain

$$
\boxed{[u]_{C^{0,\mu}(\overline{B_{1/4}})}\leq C\|u\|_{L^\infty(B_1)},
\qquad u\in C^{0,\mu}(\overline{B_{1/4}}).}
$$

The constants depend only on $n,\lambda,\Lambda$. This derives the relevant conclusion of the [De Giorgi-Nash-Moser theorem](../../../../../../de-giorgi-nash-moser-theorem.md) directly from part (a).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
