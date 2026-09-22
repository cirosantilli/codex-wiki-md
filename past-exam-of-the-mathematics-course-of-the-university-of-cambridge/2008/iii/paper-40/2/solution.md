<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In a price-taking equilibrium, market clearing fixes aggregate consumption at the dividend $\delta_t$, so $c_t^i=p_t^i\delta_t$ and $\sum_i p_t^i=1$. Each agent takes this aggregate benchmark as given when varying their own consumption. Let $\xi_t$ be a common [state-price density](../../../../../state-price-density.md) and $y_i>0$ their budget multipliers. Marginal pricing gives

$$
e^{-\rho_it}\frac{U_i'(p_t^i)}{\delta_t}=y_i\xi_t.
$$

Write $I_i=(U_i')^{-1}$ and $b_t=\xi_t\delta_t$. Then

$$
p_t^i=I_i(y_ie^{\rho_it}b_t),\qquad\sum_i I_i(y_ie^{\rho_it}b_t)=1.
$$

For fixed $t$, the second left side is continuous and strictly decreasing from infinity to zero, so it determines a unique positive number $b(t)$. Every coefficient in that equation is deterministic. Consequently

$$
\boxed{p_t^i=I_i(y_ie^{\rho_it}b(t))\text{ is deterministic},\qquad\xi_t=\frac{b(t)}{\delta_t}.}
$$

This is the [relative-consumption share equilibrium](../../../../../relative-consumption-share-equilibrium.md). The absolute consumption streams remain random through $\delta_t$.

Assuming finite fundamental prices, the ex-dividend price of the productive asset follows from conditional pricing:

$$
\boxed{S_t=\xi_t^{-1}\mathbb E_t\int_t^\infty\xi_s\delta_s\,ds
=\frac{\delta_t}{b(t)}\int_t^\infty b(s)\,ds.}
$$

The initial [state-price budget constraints](../../../../../state-price-budget-constraint.md) determine the multipliers up to a common normalization:

$$
\int_0^\infty b(t)I_i(y_ie^{\rho_it}b(t))\,dt
=\pi_0^i\int_0^\infty b(t)\,dt,\qquad i=1,\ldots,J.
$$

Together with the scalar market-clearing equation these characterize the equilibrium. A common scaling of all $y_i$ is offset by the reciprocal scaling of $b$. At least one redundant budget equation can be removed, since the initial fractions sum to one.

For completeness, define $B(t)=\int_t^\infty b(s)ds$ and $B_i(t)=\int_t^\infty b(s)p_s^i ds$. The consumption-financing wealth is $w_t^i=\delta_tB_i(t)/b(t)$. Its stochastic exposure and that of $S_t$ are both proportional to $\delta_t$. Thus holding $B_i(t)/B(t)$ units of the productive asset, with no bank-account balance, finances this wealth and consumption. Indeed, the holding's deterministic changes and dividend consumption balance because $B_i'=-bp^i$ and $B'=-b$.

If all $\rho_i=\rho$ and $U_i=U$, market clearing gives $b(t)=ke^{-\rho t}$ for a constant $k>0$, and $p_t^i=I(y_ik)$ is constant. The budget equations then imply

$$
\boxed{p_t^i=\pi_0^i,\qquad c_t^i=\pi_0^i\delta_t,\qquad S_t=\delta_t/\rho.}
$$

For differentiable $b$, the general equilibrium has short rate $r_t=\mu-\sigma^2-b'(t)/b(t)$ and risky-asset total expected return $r_t+\sigma^2$; its volatility is $\sigma$. These follow directly from $\xi_t=b(t)/\delta_t$ and the [Itô formula](../../../../../ito-s-lemma.md). In the identical-agent case, $r=\mu-\sigma^2+\rho$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
