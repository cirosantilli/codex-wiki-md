# Finite-horizon drawdown of a two-sign-memory process

↑ **Parent:** [Drawdown (economics)](drawdown-economics.md)

For increments $X_t=a_{t-2}a_{t-1}+a_t$ with freely admissible starting sign history, the worst absolute [financial drawdown](drawdown-economics.md) over $N$ steps is the displayed value. A four-state recursion $d_{n+1}(b,c)=\min_{a=\pm1}[d_n(a,b)+ab+c]$ computes the minimum cumulative increment, with zero initial costs. The minimum is attained by nonpositive increments: $(-2,0)^k,-2$ for odd $N=2k+1$, and $(-2,0)^{k-1},-2,-2$ for even $N=2k$. The horizon-free bound is infinite. At most two strictly negative increments can be consecutive, but confusing that losing-run bound with drawdown would be incorrect.

## ↑ Ancestors (6)

1. [Drawdown (economics)](drawdown-economics.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
