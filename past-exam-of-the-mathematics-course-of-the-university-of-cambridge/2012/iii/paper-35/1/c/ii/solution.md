<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $X_t=g_t(x)-W_t$, $Y_t=g_t(y)-W_t$ and $D_t=Y_t-X_t$. Before $T(x)$, order preservation gives $0<X_t<Y_t$ and $D_t>0$. The common noise cancels from their difference:

$$
dD_t=\left(\frac2{Y_t}-\frac2{X_t}\right)dt
=-\frac{2D_t}{X_tY_t}\,dt.
$$

Since $D$ has finite variation, applying the [Itô formula](../../../../../../../ito-s-lemma.md) to $Z=Y/D$ gives the [SLE two-boundary-point ratio diffusion](../../../../../../../sle-two-boundary-point-ratio-diffusion.md)

$$
\boxed{dZ_t=-\frac{\sqrt\kappa}{D_t}\,d\beta_t
+\frac2{D_t^2}\left(\frac1{Z_t}+\frac1{Z_t-1}\right)dt,\qquad Z_t>1.}
$$

With the strictly increasing clock $u(t)=\int_0^tD_s^{-2}ds$, the [Dambis-Dubins-Schwarz theorem](../../../../../../../dambis-dubins-schwarz-theorem.md) yields a [Brownian motion](../../../../../../../brownian-motion-split.md) $B$ for which the time-changed process obeys

$$
d\widehat Z_u=\sqrt\kappa\,dB_u
+2\left(\frac1{\widehat Z_u}+\frac1{\widehat Z_u-1}\right)du.
$$

The sign of the new [Brownian motion](../../../../../../../brownian-motion-split.md) has absorbed the minus sign above.

The [domain Markov property of a chordal Loewner chain](../../../../../../../domain-markov-property-of-a-chordal-loewner-chain.md) says that, conditionally on the past before $T(x)$, the mapped future is a fresh [SLE](../../../../../../../schramm-loewner-evolution.md). Its boundary marked points are $X_t,Y_t$. Hence

$$
\mathbb P(T(x)<T(y)\mid\mathcal F_t)=F(X_t,Y_t)=f(Z_t),\qquad t<T(x).
$$

Localize, for example, where $D_t\geq1/n$, $Z_t\in[1+1/n,n]$ and $t\leq n$. On each such stopped interval this is a bounded [conditional-expectation martingale](../../../../../../../conditional-expectation-martingale.md), and therefore a genuine [martingale](../../../../../../../martingale-split.md). No smoothness assumption on $f$ is needed for this argument. The exit calculation below identifies it explicitly.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
