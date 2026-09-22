<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\mathcal L_rV(s)=\frac12\sigma^2s^2V''(s)+rsV'(s)$ and define the nonnegative reserve rate $a(s)=rV(s)-\mathcal L_rV(s)$. The [obstacle problem](../../../../../../obstacle-problem.md) gives $V\geq g$ and $a\geq0$. The [American-option superhedge with a funded reserve](../../../../../../american-option-superhedge-with-a-funded-reserve.md) invests the local surplus in the bond rather than consuming it.

For initial wealth $x\geq V(S_0)$, set

$$
D_t=e^{rt}\left(x-V(S_0)+\int_0^te^{-ru}a(S_u)\,du\right),\qquad F_t=V(S_t)+D_t,
$$

and choose the [stock](../../../../../../stock.md) and bond holdings

$$
\boxed{\pi_t=V'(S_t),\qquad \phi_t=\frac{F_t-\pi_tS_t}{B_t}.}
$$

Thus $D_t\geq0$ and $F_t\geq V(S_t)\geq g(S_t)$, pathwise at every time. The [Itô formula](../../../../../../ito-s-lemma.md) under the original drift gives

$$
dV(S_t)=V'(S_t)\,dS_t+\tfrac12\sigma^2S_t^2V''(S_t)\,dt,
\qquad dD_t=(rD_t+a(S_t))\,dt.
$$

Adding these equations yields

$$
\boxed{dF_t=\pi_t\,dS_t+r(F_t-\pi_tS_t)\,dt
=\pi_t\,dS_t+\phi_t\,dB_t.}
$$

This is a [self-financing strategy](../../../../../../self-financing-portfolio.md), and its nonnegative wealth makes it an [admissible trading strategy](../../../../../../admissible-trading-strategy.md). Continuity of the [stock](../../../../../../stock.md) and local regularity of $V$ ensure local integrability of the holdings. The construction does not require $\mu=r$.

For a classical solution, the usual [Itô formula](../../../../../../ito-s-lemma.md) applies directly. The [smooth fit](../../../../../../smooth-pasting.md) solution below is $C^1$ and piecewise $C^2$, with locally absolutely continuous first derivative. The generalized [Itô formula](../../../../../../ito-s-lemma.md) applies with its almost-everywhere second derivative; the absence of a derivative jump means no boundary [local time of a semimartingale](../../../../../../local-time-of-a-semimartingale.md) term. This is the usual regularity interpretation of the perpetual [American option](../../../../../../american-option.md) obstacle equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
