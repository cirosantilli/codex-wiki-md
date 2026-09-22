<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $S>b$, maximize the coefficient $H(b)=b^\gamma(K-b)^n$ of $S^{-\gamma}$. Its logarithmic [derivative](../../../../../derivative.md) is

$$
\frac{H'(b)}{H(b)}=\frac\gamma b-\frac n{K-b}.
$$

It changes sign once, at $b=\gamma K/(\gamma+n)$. The [perpetual power put option](../../../../../perpetual-power-put-option.md) therefore has candidate value

$$
\boxed{b=\frac{2rK}{2r+n\sigma^2},\qquad V_n(S)=\begin{cases}(K-S)^n,&0\leq S\leq b,\\(K-b)^n(S/b)^{-2r/\sigma^2},&S>b.\end{cases}}
$$

The same boundary follows from [smooth fit](../../../../../smooth-pasting.md), $-\gamma(K-b)^n/b=-n(K-b)^{n-1}$. To establish optimality among all [stopping times](../../../../../stopping-time.md), rather than only fixed barriers, we verify the candidate. Let $\mathcal L=rS\partial_S+\sigma^2S^2\partial_{SS}/2$ be the [infinitesimal generator](../../../../../infinitesimal-generator-stochastic-processes.md). The maximum property of $H$ gives $V_n\geq g_n$ everywhere, and $(\mathcal L-r)V_n=0$ for $S>b$. For $S\leq b$, set $y=S/(K-S)\leq\gamma/n$. Then

$$
\frac{(\mathcal L-r)g_n}{g_n}=\frac12\sigma^2\big[n(n-1)y^2-\gamma ny-\gamma\big]\leq-r(1+y)<0.
$$

Thus the discounted candidate is a nonnegative [supermartingale](../../../../../supermartingale.md). The [smooth fit](../../../../../smooth-pasting.md) removes the derivative-jump [local time of a semimartingale](../../../../../local-time-of-a-semimartingale.md) term in the [Itô formula](../../../../../ito-s-lemma.md). The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) and localization bound every exercise policy's discounted [expected value](../../../../../expected-value-split.md) by $V_n$. Immediate exercise attains it below $b$; the first hitting time of $b$ attains it above $b$. The terminal remainder vanishes since $0\leq e^{-ru}V_n(S_u)\leq K^n e^{-ru}\to0$. This proves the displayed value.

For $n=1$ it reduces to the ordinary [perpetual put option](../../../../../perpetual-put-option.md). Larger $n$ lowers the optimal trigger, because the more strongly curved [financial payoff](../../../../../contingent-claim-payoff.md) makes further downward moves more valuable. If $r=0$, under the [risk-neutral measure](../../../../../risk-neutral-measure.md) the stock tends to zero [almost surely](../../../../../almost-sure-convergence.md), so the supremum is $K^n$, approached as the exercise time tends to infinity and not attained at a finite time when $S>0$. If $r<0$, the values at deterministic exercise times grow without bound; the perpetual value is infinite. These cases do not admit the positive-rate formula above.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../../split.md)
6. [Mathematical models of financial derivatives course of the University of Oxford](../../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
