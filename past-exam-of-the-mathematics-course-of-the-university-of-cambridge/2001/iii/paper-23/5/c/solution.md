<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose the forward field is differentiable in maturity with the stochastic integrability needed for differentiation. As time increases, both arguments of $r_t=f(t,t)$ increase. The [diagonal short-rate dynamics in the Heath-Jarrow-Morton model](../../../../../../diagonal-short-rate-dynamics-in-the-heath-jarrow-morton-model.md) are therefore

$$
dr_t=[\partial_Tf(t,t)+\alpha^Q(t,t)]dt+\sigma(t,t)dW_t^Q.
$$

Under the HJM drift restriction from part (a), $\alpha^Q(t,t)=0$, giving

$$
\boxed{dr_t=\partial_Tf(t,t)\,dt+\sigma(t,t)dW_t^Q.}
$$

More explicitly the slope is

$$
\partial_Tf(t,t)=f_0'(t)+\int_0^t\partial_T\alpha^Q(s,t)\,ds
+\int_0^t\partial_T\sigma(s,t)\,dW_s^Q.
$$

It depends on the forward curve and potentially the whole history, not necessarily on $r_t$ alone. Without the stated maturity regularity, the original forward equations do not by themselves guarantee this classical [Itô process](../../../../../../ito-process.md) formula for the diagonal.

**The [short rate](../../../../../../short-rate.md) need not be [Markov](../../../../../../markov-property.md), even with one Brownian factor and deterministic volatility.** An explicit example of [One Brownian factor does not imply a Markov short rate](../../../../../../one-brownian-factor-does-not-imply-a-markov-short-rate.md) takes $f_0(T)=0$ and $\sigma(t,T)=T-t$. Its no-arbitrage forward drift is $\alpha^Q(t,T)=(T-t)^3/2$, so

$$
r_t=\frac{t^4}{8}+\int_0^t(t-s)dW_s
=\frac{t^4}{8}+I_t,\qquad I_t=\int_0^tW_sds.
$$

The continuous rate history determines $W_t$ from the left [derivative](../../../../../../derivative.md) of $I_t$. Hence for $h>0$,

$$
\mathbb E[I_{t+h}\mid\mathcal F_t^r]=I_t+hW_t.
$$

But $W_t$ is not determined by $I_t$: joint normality, $\operatorname{Var}I_t=t^3/3$, and $\operatorname{Cov}(W_t,I_t)=t^2/2$ give

$$
\operatorname{Var}(W_t\mid I_t)=t-\frac{(t^2/2)^2}{t^3/3}=\frac t4>0.
$$

Thus the conditional mean of the future given the whole rate history cannot be a function of the current rate alone, contradicting the [Markov property](../../../../../../markov-property.md). Enlarging the state to $(I_t,W_t)$ gives a two-dimensional [Markov process](../../../../../../markov-process-split.md); special HJM specifications can instead close on a single [short rate](../../../../../../short-rate.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
