<h1 id="3/2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Put $h=|u-v|$, $q=Q(u,v)$ and $h_0=|u_0-v_0|$. The [mean value theorem](../../../../../../../mean-value-theorem.md) gives $|q|\le Mh$ on the bounded state range. Fix a final time $t$ and let $L(\tau)=a-M(t-\tau)$ and $R(\tau)=b+M(t-\tau)$. Choose a smooth increasing function $\rho$ equal to zero on $(-\infty,0]$ and one on $[1,\infty)$. For small $\delta>0$, define

$$
W_\delta(\tau,x)=\rho\left(\frac{x-L(\tau)}\delta\right)\rho\left(\frac{R(\tau)-x}\delta\right).
$$

Its two nonnegative [derivative](../../../../../../../derivative.md) contributions imply $(W_\delta)_\tau+M|(W_\delta)_x|\le0$. Therefore $h(W_\delta)_\tau+q(W_\delta)_x\le0$.

Use the nonnegative test $\varphi(\tau,x)=\eta_\epsilon(\tau)W_\delta(\tau,x)$, where $\eta_\epsilon(0)=1$, it is one up to just before $s$, decreases smoothly to zero near $s$, and remains zero afterward. The [Kato inequality for scalar conservation laws](../../../../../../../kato-inequality-for-scalar-conservation-laws.md) gives

$$
-\int\eta_\epsilon'(\tau)\!\int hW_\delta\,dx\,d\tau\le\int h_0(x)W_\delta(0,x)\,dx,
$$

because the other interior contribution is nonpositive. At Lebesgue times $s$, the temporal [approximate identity](../../../../../../../approximate-identity.md) tends to $\int h(s)W_\delta(s)$; take a countable sequence $\delta\downarrow0$ and use dominated convergence on the bounded cone. This yields

$$
\boxed{\int_{a-M(t-s)}^{b+M(t-s)}|u(s,x)-v(s,x)|dx\le\int_{a-Mt}^{b+Mt}|u_0(x)-v_0(x)|dx}
$$

for almost every $s\in[0,t]$. This is [local L1 contraction for scalar conservation laws](../../../../../../../local-l1-contraction-for-scalar-conservation-laws.md). It uses only local integrability, so the bounded data need not have finite global $L^1$ [norm](../../../../../../../norm.md). If $M=0$, the flux difference is zero and the same proof uses a stationary interval.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
