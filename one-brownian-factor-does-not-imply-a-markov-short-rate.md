# One Brownian factor does not imply a Markov short rate

↑ **Parent:** [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)

For the [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md) with $\sigma(t,T)=T-t$, the risk-neutral drift is $\alpha(t,T)=(T-t)^3/2$. Its [short rate](short-rate.md) is $r_t=f(0,t)+t^4/8+\int_0^tW_sds$. The centered integrated Brownian component is not [Markov](markov-property.md): its past reveals its derivative $W_t$, which affects the conditional mean of future increments, whereas its current integral does not determine $W_t$. Indeed the conditional variance of $W_t$ given the current integral is $t/4$. A one-dimensional driving noise therefore does not force a one-dimensional Markov state.

## ↑ Ancestors (8)

1. [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)
2. [Interest rate](interest-rate.md)
3. [Fixed-income security](fixed-income-security.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48/4/c/solution.md)
