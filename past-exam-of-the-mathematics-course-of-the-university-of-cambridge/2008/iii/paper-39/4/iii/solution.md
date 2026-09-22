<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\phi$ denote the standard [Gaussian distribution](../../../../../../normal-distribution.md) [probability density function](../../../../../../probability-density-function.md). Directly from the definitions, $S\phi(d_1)=Ke^{-r\tau}\phi(d_2)$. Differentiating the price in part (ii), the terms involving [derivatives](../../../../../../derivative.md) of $d_1,d_2$ cancel, yielding $V_S=\Phi(d_1)$. Therefore, in units of the two traded assets, the [replicating strategy](../../../../../../replicating-strategy.md) is

$$
\boxed{h^S_t=\Phi(d_1),\qquad h^B_t=\frac{Ke^{-r(T-t)}\Phi(-d_2)}{B_t}\qquad(t<T).}
$$

Its value is $h^B_tB_t+h^S_tS_t=V(t,S_t)$. To check self-financing explicitly, [differentiation](../../../../../../differentiation.md) also gives

$$
V_{SS}=\frac{\phi(d_1)}{S\sigma\sqrt\tau},\qquad V_t=-\frac{S\sigma\phi(d_1)}{2\sqrt\tau}+rKe^{-r\tau}\Phi(-d_2).
$$

Hence $V_t+rSV_S+\tfrac12\sigma^2S^2V_{SS}=rV$. Applying [Itô formula](../../../../../../ito-s-lemma.md) under the physical measure gives

$$
dV=[rV+(\mu-r)SV_S]dt+\sigma SV_SdW=h^B_t\,dB_t+h^S_t\,dS_t.
$$

Thus the holdings form a [self-financing strategy](../../../../../../self-financing-portfolio.md) and their terminal value is the required payout. Holdings at the single maturity instant can be assigned by their limiting values; the continuous-time trading gains do not depend on that assignment. If $\pi_t$ denotes wealth fractions instead, the stock fraction is $S_t\Phi(d_1)/V(t,S_t)$ and the bank fraction is $Ke^{-r\tau}\Phi(-d_2)/V(t,S_t)$. For $K\leq0$, hold one stock and no bank-account units.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
