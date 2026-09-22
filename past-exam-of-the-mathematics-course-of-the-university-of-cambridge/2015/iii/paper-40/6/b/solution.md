<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiating the [European call option](../../../../../../european-call-option.md) price in strike gives, for $T>0$,

$$
C_K(T,K)=-e^{-rT}\int_K^\infty\psi(T,s)\,ds,
\qquad C_{KK}(T,K)=e^{-rT}\psi(T,K).
$$

The strike derivative uses dominated convergence; the second uses the continuous density. Also,

$$
\int_K^\infty s\psi(T,s)\,ds
=e^{rT}\bigl(C(T,K)-KC_K(T,K)\bigr).
$$

Differentiate the supplied time-integral identity and the discount factor. Continuity of the density supplies the diffusion-term derivative. For the tail first moment, continuity in time follows from continuous [stock](../../../../../../stock.md) paths, locally uniformly bounded second moments, and the absence of an atom at $K$. Therefore

$$
\begin{aligned}
C_T&=-rC+e^{-rT}\left(r\int_K^\infty s\psi(T,s)\,ds
+\frac12K^2\sigma(T,K)^2\psi(T,K)\right)\\
&=-rKC_K+\frac12K^2\sigma(T,K)^2C_{KK}.
\end{aligned}
$$

Hence the [Dupire equation](../../../../../../dupire-equation.md) is

$$
\boxed{C_T(T,K)=\frac12K^2\sigma(T,K)^2C_{KK}(T,K)-rKC_K(T,K).}
$$

Its initial condition is $C(0,K)=(S_0-K)^+$; natural strike boundaries are $C(T,0)=S_0$ and $C(T,K)\to0$ as $K\to\infty$. These are consistent with the discounted [stock](../../../../../../stock.md) [martingale](../../../../../../martingale-split.md) and integrable tails. Where $C_{KK}>0$, the same identity gives [local volatility recovery from call prices](../../../../../../local-volatility-recovery-from-call-prices.md):

$$
\boxed{\sigma(T,K)^2=
\frac{2(C_T+rKC_K)}{K^2C_{KK}}.}
$$

The equation evolves in maturity and strike, unlike the backward option-value equation in calendar time and spot.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
