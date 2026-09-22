<h1 id="m/m4/solution">Solution</h1>

↑ **Parent:** [M4](../m4.md)

The [central limit theorem](../../../../central-limit-theorem.md) states that for independent identically distributed variables of finite mean $\mu$ and positive finite [variance](../../../../variance-split.md) $\sigma^2$,

$$
\frac{\sum_{j=1}^nX_j-n\mu}{\sigma\sqrt n}\xrightarrow d N(0,1).
$$

For a continuous strictly increasing [cumulative distribution function](../../../../cumulative-distribution-function.md), its inverse is defined on $(0,1)$. Thus $\mathbb P(F(X)\le y)=\mathbb P(X\le F^{-1}(y))=y$ for $0<y<1$, proving the uniform law.

If $T=-\log(1-Y)$, then for $t\ge0$, $\mathbb P(T\le t)=\mathbb P(Y\le1-e^{-t})=1-e^{-t}$. Hence $f_T(t)=e^{-t}\mathbf1_{(0,\infty)}(t)$, an exponential density of rate one. Its first two moments are one and two, by [integration by parts](../../../../integration-by-parts.md), so $\mathbb ET=1$ and $\operatorname{Var}T=1$.

Although the original variables may have different distributions, their separate transforms $Y_k=F_k(X_k)$ are independent and all uniform. Consequently $T_k=-\log(1-Y_k)$ are independent identically distributed exponentials of rate one, and the statistic is exactly

$$
Z_n=\frac{\sum_{k=1}^nT_k-n}{\sqrt n}.
$$

The stated [central limit theorem](../../../../central-limit-theorem.md) therefore yields $\boxed{Z_n\xrightarrow d N(0,1)}$.

## ↑ Ancestors (12)

1. [M4](../m4.md)
2. [M](../../m.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
