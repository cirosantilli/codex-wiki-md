# Diagonal short-rate dynamics in the Heath-Jarrow-Morton model

↑ **Parent:** [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)

For a maturity-differentiable [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md) forward field with the integrability needed for stochastic differentiation, the [short rate](short-rate.md) $r_t=f(t,t)$ has the displayed dynamics. Indeed changing observation time uses the forward-rate [stochastic differential equation](stochastic-differential-equation.md), while changing maturity adds $\partial_Tf(t,t)dt$. Under a [risk-neutral measure](risk-neutral-measure.md), $\alpha(t,T)=\sigma(t,T)\int_t^T\sigma(t,u)du$, so $\alpha(t,t)=0$. The remaining drift depends on the diagonal slope of the whole forward curve, which need not be determined by $r_t$; a [Markov process](markov-process-split.md) for the [short rate](short-rate.md) is an additional modelling restriction. Without sufficient maturity regularity, the diagonal need not admit this classical [Itô process](ito-process.md) formula.

## ↑ Ancestors (8)

1. [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)
2. [Interest rate](interest-rate.md)
3. [Fixed-income security](fixed-income-security.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/5/c/solution.md)
