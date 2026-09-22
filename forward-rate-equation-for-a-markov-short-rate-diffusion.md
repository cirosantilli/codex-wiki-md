# Forward-rate equation for a Markov short-rate diffusion

↑ **Parent:** [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)

Suppose $dr_t=a(r_t)dt+b(r_t)dW_t$ under a risk-neutral measure and $f_t(T)=F(T-t,r_t)$. By [Itô formula](ito-s-lemma.md), the forward-rate volatility is $\sigma_t(T)=b(r_t)F_r(T-t,r_t)$. The [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md) drift restriction is equivalent to

$$
F_\theta=aF_r+\frac12b^2F_{rr}-b^2F_r\int_0^\theta F_r(s,r)ds,\qquad F(0,r)=r.
$$

To verify it directly for bonds, put $G(\theta,r)=\int_0^\theta F(s,r)ds$. Integration gives $F-r=aG_r+\tfrac12b^2G_{rr}-\tfrac12b^2G_r^2$. The [zero-coupon bond](zero-coupon-bond.md) price $P(t,T)=e^{-G(T-t,r_t)}$ therefore satisfies

$$
\frac{dP(t,T)}{P(t,T)}=r_tdt-b(r_t)G_r(T-t,r_t)dW_t.
$$

Its bank-account-discounted price is a positive [local martingale](local-martingale.md). A common equivalent [local martingale](local-martingale.md) measure excludes admissible [arbitrage](arbitrage.md) for any finite collection of these traded maturities.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32/6/solution.md)
