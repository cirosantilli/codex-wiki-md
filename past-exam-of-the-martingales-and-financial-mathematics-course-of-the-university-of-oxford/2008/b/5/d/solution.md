<h1 id="b/5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $F(t,s)$ be the ordinary Black-Scholes price of the terminal claim $G(S_T)$. Denote the new asset by $U_t=a(t)S_t^2$. Since it is strictly increasing in $S_t>0$, invert it as $s=\sqrt{U/a(t)}$ and write $H(t,U)=F(t,\sqrt{U/a(t)})$. Its derivative is

$$
H_U=\frac{sF_s}{2U}.
$$

The [replicating portfolio](../../../../../replicating-strategy.md) in the new asset and bank account therefore holds

$$
\boxed{\Gamma_t=\frac{S_tF_s(t,S_t)}{2U_t},\qquad
\beta_t=\frac{F(t,S_t)-\tfrac12S_tF_s(t,S_t)}{B_t}.}
$$

The wealth is $F$. The diffusion coefficient of $\Gamma\,dU$ is $2\sigma U\Gamma=\sigma SF_s$, agreeing with that of $dF$. Its drift together with the bank holding is

$$
(2\mu-r)\Gamma U+r\beta B
=\mu SF_s+r(F-SF_s),
$$

which equals the drift of $F$ by its Black-Scholes equation. This verifies self financing and terminal replication. Thus the square-payoff claim has nonzero volatility and can replace the original stock as the traded risky asset.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
