<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $T=t_0$ and $b(t)=e^{-\rho(T-t)}$ for the price of the unit [zero-coupon bond](../../../../../zero-coupon-bond.md) maturing at $T$, so $db=\rho b\,dt$. Let the [stock](../../../../../stock.md) satisfy $dS_t=\mu S_tdt+\sigma S_tdW_t$ with $\sigma>0$. Assume the value function $f(x,t)=xg(x,t)+b(t)h(x,t)$ is $C^{2,1}$ and the holdings have enough smoothness for the calculations below. The [self-financing portfolio](../../../../../self-financing-portfolio.md) condition is the gain identity

$$
df(S_t,t)=g(S_t,t)\,dS_t+h(S_t,t)\,db(t).
$$

The [Itô formula](../../../../../ito-s-lemma.md) expresses the left side as

$$
\left(f_t+\mu x f_x+\tfrac12\sigma^2x^2f_{xx}\right)dt+\sigma x f_x\,dW_t.
$$

Matching the diffusion terms gives $f_x=g$, or $xg_x+bh_x=0$. Differentiating $f_x=g$ gives $f_{xx}=g_x$. Also $f_t=xg_t+bh_t+\rho bh$. Matching the remaining drift terms consequently gives the two necessary conditions

$$
\boxed{xg_x+bh_x=0,\qquad xg_t+bh_t+\tfrac12\sigma^2x^2g_x=0.}
$$

They are sufficient because substituting them into the [Itô formula](../../../../../ito-s-lemma.md) restores exactly the gain identity. Necessity first holds along the [stock](../../../../../stock.md) process; its positive lognormal density for every $t>0$, together with continuity of the coefficient functions, gives the displayed identities for all $x>0$ and $0<t<T$, and continuity extends them to the endpoints.

Equivalently, the smooth value of any [self-financing portfolio](../../../../../self-financing-portfolio.md) satisfies the [Black-Scholes equation](../../../../../black-scholes-equation.md)

$$
\boxed{f_t+\rho x f_x+\tfrac12\sigma^2x^2f_{xx}-\rho f=0.}
$$

Indeed, the gain identity after imposing $g=f_x$ has drift $\mu x f_x+\rho(f-xf_x)$, which gives this equation. Conversely, if $f$ satisfies this equation, take

$$
g(x,t)=f_x(x,t),\qquad h(x,t)=\frac{f(x,t)-xf_x(x,t)}{b(t)}.
$$

The [Itô formula](../../../../../ito-s-lemma.md) then verifies that these holdings form a [self-financing portfolio](../../../../../self-financing-portfolio.md) of value $f$. This converse asserts existence of the correct holdings. It does not certify an arbitrary decomposition of $f$ into stock and bond holdings: for example, $f=0$, $g=1$, $h=-x/b$ solves the value equation but fails $g=f_x$. The [Black-Scholes value equation needs delta-compatible holdings](../../../../../black-scholes-value-equation-needs-delta-compatible-holdings.md) precisely for this reason.

For a [constant-proportion portfolio](../../../../../constant-proportion-portfolio.md), the stock value must satisfy $xg=\gamma f$. Since $g=f_x$, integration of $xf_x=\gamma f$ gives $f(x,t)=C(t)x^\gamma$. Substituting into the [Black-Scholes equation](../../../../../black-scholes-equation.md) gives

$$
C'(t)=(1-\gamma)(\rho+\tfrac12\gamma\sigma^2)C(t).
$$

Thus, for initial [portfolio wealth](../../../../../portfolio-wealth.md) $V_0$ and stock price $S_0$, the complete explicit solution is

$$
\boxed{V_t=V_0\left(\frac{S_t}{S_0}\right)^\gamma e^{(1-\gamma)(\rho+\gamma\sigma^2/2)t},\quad g_t=\frac{\gamma V_t}{S_t},\quad h_t=\frac{(1-\gamma)V_t}{b(t)}.}
$$

Here $g_t$ counts shares and $h_t$ counts maturity-$T$ bonds; the initial cost is $V_0$. Directly, the [self-financing](../../../../../self-financing-portfolio.md) gain equation is $dV_t/V_t=[\rho+\gamma(\mu-\rho)]dt+\gamma\sigma dW_t$, which also verifies the displayed value. Constant proportions concern the values of the holdings, not constant numbers of shares or bonds. The nondegenerate volatility assumption is necessary for the preceding diffusion matching; with $\sigma=0$, one only obtains a gain condition along the deterministic stock path.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
