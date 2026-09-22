<h1 id="28j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here $U'(x)=x^{-R}>0$ and $U''(x)=-Rx^{-R-1}<0$: the specified utility is [strictly concave](../../../../../../strictly-concave-function.md), contrary to the word “convex” in part (i). Assume its expected values are finite on the admissible set. Define $G_\theta=r+\theta(X-r)$ and choose a constant [portfolio](../../../../../../investment-portfolio.md) fraction $\theta_*$ maximizing $E[U(G_\theta)]$. Equivalently maximize $E[G_\theta^{1-R}]$ for $0<R<1$ and minimize it for $R>1$. An interior optimum satisfies

$$
\boxed{E[(X-r)G_{\theta_*}^{-R}]=0.}
$$

For a constrained endpoint optimum the corresponding derivative has the appropriate one-sided sign. The objective is concave in $\theta$ and [strictly concave](../../../../../../strictly-concave-function.md) if $P(X\ne r)>0$, so this condition or its endpoint version determines the optimum. Put $\kappa=E[G_{\theta_*}^{1-R}]$ and $\gamma=\kappa^{1/R}>0$.

Backward induction with [independence](../../../../../../independent-random-variables.md) of the returns gives $V_n(w)=A_nw^{1-R}/(1-R)$ and $A_N=1$. Maximizing the [consumption](../../../../../../consumption.md) expression

$$
\frac{c^{1-R}+A_{n+1}\kappa(w-c)^{1-R}}{1-R}
$$

gives $c^{-R}=A_{n+1}\kappa(w-c)^{-R}$, hence

$$
c_n^*=\frac{w_n}{1+(A_{n+1}\kappa)^{1/R}},\qquad
A_n=\big[1+(A_{n+1}\kappa)^{1/R}\big]^R.
$$

Writing $b_n=A_n^{1/R}$ yields $b_N=1$ and $b_n=1+\gamma b_{n+1}$. Therefore the fully explicit horizon dependence is

$$
\boxed{b_n=\sum_{j=0}^{N-n}\gamma^j,\qquad
c_n^*=\frac{w_n}{b_n},\qquad\theta_n^*=\theta_*.}
$$

Use $b_n=(1-\gamma^{N-n+1})/(1-\gamma)$ when $\gamma\ne1$, and $b_n=N-n+1$ when $\gamma=1$. The investor consumes this fraction, invests the remaining wealth with the same optimal [portfolio](../../../../../../investment-portfolio.md) mix at each date, and consumes all remaining wealth at $N$. If the stock is identical to the bank almost surely, every [portfolio](../../../../../../investment-portfolio.md) fraction is equivalent.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
