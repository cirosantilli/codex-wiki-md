<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [martingale](../../../../../../martingale-split.md) with the specified terminal value must equal its [conditional expectation](../../../../../../conditional-expectation.md). If $\widehat S_t=0$, [default](../../../../../../credit-default.md) has already occurred and the terminal [European call option](../../../../../../european-call-option.md) payoff is zero. If $\widehat S_t>0$, put $h=T-t$. Conditional on survival to $T$,

$$
\widehat S_T=\widehat S_t e^{\lambda h}
  \exp\{-\sigma^2h/2+\sigma\sqrt h\,Y\},
$$

where $Y$ has the [standard normal distribution](../../../../../../standard-normal-distribution.md); the [conditional probability](../../../../../../conditional-probability.md) of this survival is $e^{-\lambda h}$. The [conditional expectation](../../../../../../conditional-expectation.md) of the payoff in the enlarged [filtration](../../../../../../filtration-probability-theory.md) used in part (c) is consequently

$$
e^{-\lambda h}\widehat S_t e^{\lambda h}
 F\left(\sigma^2h,\frac{Ke^{-\lambda h}}{\widehat S_t}\right).
$$

This expression is already measurable with respect to the [natural filtration](../../../../../../natural-filtration.md) of $\widehat S$, so the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives the same value there. **The survival factor cancels the compensating growth factor**:

$$
\boxed{\widehat C_t=
\begin{cases}
\widehat S_t F\!\left(\sigma^2(T-t),\dfrac{Ke^{-\lambda(T-t)}}{\widehat S_t}\right),&\widehat S_t>0,\\
0,&\widehat S_t=0.
\end{cases}}
$$

The separate zero branch avoids division by zero. At $t=T$ it gives the required payoff, using $F(0,m)=(1-m)^+$; [integrability](../../../../../../integrability.md) follows from $(\widehat S_T-K)^+\leq\widehat S_T$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
