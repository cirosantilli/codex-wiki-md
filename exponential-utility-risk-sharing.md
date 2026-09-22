# Exponential-utility risk sharing

↑ **Parent:** [Constant absolute risk aversion utility](constant-absolute-risk-aversion-utility.md)

With positive welfare weights $a_j$, maximize $\sum_ja_j\beta_j^t[-e^{-\gamma_jc_j}/\gamma_j]$ subject to $\sum_jc_j=d$. Interior [first-order conditions](first-order-optimality-condition.md) give $a_j\beta_j^te^{-\gamma_jc_j}=\nu$. Put $\Gamma=(\sum_j\gamma_j^{-1})^{-1}$, $\log\bar\beta=\Gamma\sum_j\gamma_j^{-1}\log\beta_j$ and $\log A=\Gamma\sum_j\gamma_j^{-1}\log a_j$. Then

$$
\nu=A\bar\beta^te^{-\Gamma d},\qquad
c_j=\frac\Gamma{\gamma_j}d+\frac{t}{\gamma_j}(\log\beta_j-\log\bar\beta)+\frac1{\gamma_j}(\log a_j-\log A).
$$

If [consumption](consumption.md) must be nonnegative, the interior formula is replaced by $c_j=\max\{0,(\log a_j+t\log\beta_j-\log\nu)/\gamma_j\}$, with $\nu$ determined by resource clearing. These are Pareto allocations; realizing them as a [competitive equilibrium with one productive asset](competitive-equilibrium-with-one-productive-asset.md) requires feasible financing. For common $\beta_j=\beta$ and initial ownership $\Gamma/\gamma_j$, constant holdings and $C_t^j=(\Gamma/\gamma_j)d_t$ give such an equilibrium whenever fundamental prices and the utility sums are finite.

## ↑ Ancestors (7)

1. [Constant absolute risk aversion utility](constant-absolute-risk-aversion-utility.md)
2. [Utility function](utility-function-split.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40/1/ii/solution.md)
