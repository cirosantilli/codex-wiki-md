<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In a [complete market](../../../../../../complete-market.md), terminal-wealth optimization can first be solved over terminal payoffs and then implemented by replication. Let initial wealth be $x_0>0$, and take an increasing differentiable strictly [concave](../../../../../../concave-function.md) [utility function](../../../../../../utility-function-split.md) $U$ on $(0,\infty)$ satisfying the [Inada conditions](../../../../../../inada-conditions.md). The [state-price budget constraint](../../../../../../state-price-budget-constraint.md) for a terminal wealth $X$ is $\mathbb E_P[\zeta_nX]\leq x_0$. Monotonicity spends the whole budget at the optimum.

Let $I=(U')^{-1}$ be the [inverse marginal utility](../../../../../../inverse-marginal-utility.md). Choose $y>0$ to satisfy $\mathbb E_P[\zeta_n I(y\zeta_n)]=x_0$. In a finite tree with positive state probabilities, this left side is continuous and strictly decreasing from infinity to zero, so $y$ exists uniquely. The [complete-market terminal utility optimizer](../../../../../../complete-market-terminal-utility-optimizer.md) is

$$
\boxed{X^*=I(y\zeta_n).}
$$

To prove optimality, concavity gives $U(X)\leq U(X^*)+U'(X^*)(X-X^*)=U(X^*)+y\zeta_n(X-X^*)$. Taking expectations and using the budget proves $\mathbb EU(X)\leq\mathbb EU(X^*)$. Strict concavity gives uniqueness of the optimal terminal wealth. The finite-market setting avoids additional infinite-state existence and integrability issues.

Replicate $X^*$ using the backward recursion of part (i). Its wealth process is $V_k=B_k\mathbb E_Q[X^*/B_n\mid\mathcal F_k]$, and the two-successor difference quotient gives its [stock](../../../../../../stock.md) holdings. This [self-financing strategy](../../../../../../self-financing-portfolio.md) starts with $x_0$ by the budget equality and remains positive at every node, since it is the discounted conditional expectation of a strictly positive terminal wealth.

For logarithmic utility, $U(x)=\log x$, $I(z)=1/z$, the multiplier is $y=1/x_0$ and $X^*=x_0/\zeta_n=x_0B_n/L_n$. For [CRRA utility](../../../../../../constant-relative-risk-aversion-utility.md) with risk aversion $\gamma>0$, $\gamma\neq1$, the normalized payoff is

$$
\boxed{X^*=\frac{x_0\zeta_n^{-1/\gamma}}{\mathbb E_P[\zeta_n^{1-1/\gamma}]}.}
$$

Constraints such as prohibiting short sales change the attainable terminal-payoff set and require a constrained optimization; the unconstrained complete-market formula uses the stated assumptions.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
