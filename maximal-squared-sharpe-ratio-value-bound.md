# Maximal squared Sharpe ratio value bound

↑ **Parent:** [Merton consumption-investment problem](merton-consumption-investment-problem.md)

For $0<R<1$, common constant interest and volatility, and observed excess drift bounded in absolute value by $b_+>0$, let $V_+$ be the finite [Merton consumption-investment problem](merton-consumption-investment-problem.md) value for excess drift $b_+$. In its [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md), optimizing the stock holding contributes $-b^2(V_+')^2/(2\sigma^2V_+'')$. Since $V_+''<0$, this contribution increases with $b^2$. Thus every admissible policy makes accumulated discounted [CRRA utility](constant-relative-risk-aversion-utility.md) plus discounted $V_+$ a nonnegative [local supermartingale](local-supermartingale.md), hence a [supermartingale](supermartingale.md). Dropping its nonnegative terminal term and using the [monotone convergence theorem](monotone-convergence-theorem.md) proves the value bound. The condition $[\rho-(1-R)(r+b_+^2/(2R\sigma^2))]/R>0$ is essential for the finite supermartingale construction.

## ↑ Ancestors (10)

1. [Merton consumption-investment problem](merton-consumption-investment-problem.md)
2. [Investment-consumption problem](investment-consumption-problem.md)
3. [Expected utility maximization](expected-utility-maximization.md)
4. [Expected utility hypothesis](expected-utility-hypothesis.md)
5. [Utility function](utility-function-split.md)
6. [Mathematical finance](mathematical-finance-split.md)
7. [Mathematical optimization](mathematical-optimization-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39/4/ii/solution.md)
