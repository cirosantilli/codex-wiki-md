<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\tau=T-t$. The [product rule](../../../../product-rule.md) and [Itô's formula](../../../../ito-s-lemma.md) give

$$
\begin{aligned}
d\bigl(e^{r(T-t)}V(S_t,t)\bigr)
&=e^{r\tau}\left[V_t+\frac12\sigma^2S_t^2V_{SS}+rS_tV_S-rV\right]dt
+e^{r\tau}\sigma S_tV_S\,dW_t\\
&=e^{r\tau}\sigma S_tV_S\,dW_t,
\end{aligned}
$$

where the [Black-Scholes equation](../../../../black-scholes-equation.md) cancels the drift. Under the usual pricing growth and integrability conditions this [local martingale](../../../../local-martingale.md) is a [martingale](../../../../martingale-split.md). Its terminal value is $f(S_T)$, since the exponential factor becomes one at $T$. Taking a [conditional expectation](../../../../conditional-expectation.md) gives

$$
e^{r(T-t)}V(S_t,t)=\mathbb E[f(S_T)\mid\mathcal F_t],\qquad
\boxed{V(S,t)=e^{-r(T-t)}\mathbb E[f(S_T)\mid S_t=S].}
$$

The dynamics already use the [risk-neutral measure](../../../../risk-neutral-measure.md). This is the [Feynman-Kac formula](../../../../feynman-kac-formula.md) for the given pricing problem; a differential equation alone, without the relevant growth condition, would not justify upgrading a local martingale or uniqueness.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
