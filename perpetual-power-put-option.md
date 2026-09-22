# Perpetual power put option

↑ **Parent:** [Power put option](power-put-option.md)

For a dividend-free [Black-Scholes model](black-scholes-model.md) with $r>0$, $\sigma>0$, $K>0$ and positive [integer](integer-split.md) $n$, the [optimal stopping](optimal-stopping.md) value of the [power put option](power-put-option.md) is

$$
V(S)=\begin{cases}(K-S)^n,&0\leq S\leq b,\\(K-b)^n(S/b)^{-\gamma},&S>b,\end{cases}\qquad \gamma=\frac{2r}{\sigma^2},\quad b=\frac{\gamma K}{\gamma+n}.
$$

In the continuation region the stationary [Black-Scholes equation](black-scholes-equation.md) has powers $S$ and $S^{-\gamma}$. Boundedness at infinity removes $S$. Value matching gives the coefficient $(K-b)^nb^\gamma$, maximized at the displayed $b$; equivalently this is the [smooth fit](smooth-pasting.md) boundary.

For a verification beyond constant-trigger policies, let $g(S)=(K-S)_+^n$. The maximum property of $b^\gamma(K-b)^n$ gives $V\geq g$. For the [infinitesimal generator](infinitesimal-generator-stochastic-processes.md) $\mathcal L=rS\partial_S+\sigma^2S^2\partial_{SS}/2$, $(\mathcal L-r)V=0$ above $b$. Below $b$, set $y=S/(K-S)\leq\gamma/n$; then

$$
\frac{(\mathcal L-r)g}{g}=\frac12\sigma^2[n(n-1)y^2-\gamma ny-\gamma]\leq-r(1+y)<0.
$$

The candidate is continuously differentiable across $b$, so the generalized [Itô formula](ito-s-lemma.md) has no derivative-jump [local time of a semimartingale](local-time-of-a-semimartingale.md) term. The discounted candidate is a nonnegative [supermartingale](supermartingale.md), bounding every stopping reward by [optional stopping](optional-sampling-theorem-for-a-supermartingale.md). First hitting of $b$ attains the bound; the remainder at infinite time vanishes since $V\leq K^n$ and $r>0$. For $n=1$ this recovers the [perpetual put option](perpetual-put-option.md). At $r=0$ the value is $K^n$ for $S>0$, approached but not attained at a finite exercise time. At $r<0$ the perpetual value is infinite, because exercise at deterministic times tending to infinity has unbounded discounted [expected value](expected-value-split.md).

## ↑ Ancestors (9)

1. [Power put option](power-put-option.md)
2. [Put option](put-option.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2023/2/b/iii/solution.md)
- [Power put option](power-put-option.md)
