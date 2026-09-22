# Black-Scholes digital option formula

↑ **Parent:** [Black-Scholes model](black-scholes-model.md)

In the [Black-Scholes model](black-scholes-model.md), a [digital call option](digital-call-option.md) and [digital put option](digital-put-option.md) with remaining maturity $\tau$ have values

$$
D_{\rm call}(t,S)=e^{-r\tau}\Phi(d_-),
\qquad
D_{\rm put}(t,S)=e^{-r\tau}\Phi(-d_-),
$$

where $d_-$ is defined in the [Black-Scholes formula](black-scholes-formula.md). For $t<T$, the digital-call [delta hedge](delta-hedge.md) is

$$
\partial_SD_{\rm call}(t,S)
=\frac{e^{-r\tau}\phi(d_-)}{S\sigma\sqrt\tau}.
$$

**Table of contents**

- [Digital put-call parity](digital-put-call-parity.md)

## ↑ Ancestors (6)

1. [Black-Scholes model](black-scholes-model.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4/28j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/29k/b/solution.md)
