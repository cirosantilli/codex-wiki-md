# Normalized Black-Scholes call function

↑ **Parent:** [Black-Scholes formula](black-scholes-formula.md)

For $v,m\geq0$, define $F(v,m)=\mathbb E[(e^{-v/2+\sqrt vY}-m)^+]$, where $Y$ has the [standard normal distribution](standard-normal-distribution.md). For $v,m>0$, completing the square in the [standard normal density](standard-normal-density.md) gives

$$
F(v,m)=\Phi(d_1)-m\Phi(d_2),\qquad d_1=\frac{-\log m+v/2}{\sqrt v},\quad d_2=d_1-\sqrt v,
$$

where $\Phi$ is the [standard normal distribution function](standard-normal-distribution-function.md). The boundary values are $F(0,m)=(1-m)^+$ and $F(v,0)=1$. Multiplying by the current [stock](stock.md) price produces a zero-interest [Black-Scholes formula](black-scholes-formula.md) with total variance $v$ and relative strike $m$.

## ↑ Ancestors (7)

1. [Black-Scholes formula](black-scholes-formula.md)
2. [Black-Scholes model](black-scholes-model.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211/1/b/solution.md)
- [Put-call symmetry in the Black-Scholes model](put-call-symmetry-in-the-black-scholes-model.md)
