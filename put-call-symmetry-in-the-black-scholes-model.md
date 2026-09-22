# Put-call symmetry in the Black-Scholes model

↑ **Parent:** [Put-call parity](put-call-parity.md)

For the [normalized Black-Scholes call function](normalized-black-scholes-call-function.md), completing the square gives $F(v,m)=\Phi(d_1)-m\Phi(d_2)$, with $d_1=(-\log m+v/2)/\sqrt v$ and $d_2=d_1-\sqrt v$. The identities $d_1(v,1/m)=-d_2(v,m)$ and $\Phi(-x)=1-\Phi(x)$ imply

$$
F(v,m)=1-m+mF(v,1/m).
$$

For a [stock](stock.md) with risk-neutral drift $r$, maturity difference $\tau$, and positive strike $K$, [put-call parity](put-call-parity.md) then gives

$$
P_t(T,K)=Ke^{-r\tau}F\left(\sigma^2\tau,\frac{S_te^{r\tau}}K\right).
$$

The positive sign of $r\tau$ in the reciprocal argument is forced by taking the reciprocal of $Ke^{-r\tau}/S_t$. The identity includes $v=0$ by continuity and requires $m>0$.

## ↑ Ancestors (8)

1. [Put-call parity](put-call-parity.md)
2. [European call option](european-call-option.md)
3. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/28j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32/5/solution.md)
