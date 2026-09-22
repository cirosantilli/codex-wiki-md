<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $X=e^\beta\cos\theta$ and $Y=e^\beta\sin\theta$, apply the two-variable [Itô formula](../../../../../../ito-s-lemma.md). Independence gives $[\beta,\theta]=0$, while each individual bracket is $t$. The second derivatives in the two variables cancel, yielding

$$
\boxed{dX_t=X_t\,d\beta_t-Y_t\,d\theta_t,\qquad dY_t=Y_t\,d\beta_t+X_t\,d\theta_t.}
$$

Their integrands are continuous adapted and locally bounded, so both coordinates are [continuous local martingales](../../../../../../continuous-local-martingale.md). The [quadratic variation of a stochastic integral](../../../../../../quadratic-variation-of-a-stochastic-integral.md) gives

$$
\boxed{[X]_t=[Y]_t=A_t:=\int_0^t(X_s^2+Y_s^2)ds=\int_0^te^{2\beta_s}ds,\qquad[X,Y]_t=\int_0^t(X_sY_s-Y_sX_s)ds=0.}
$$

Here is a full proof that the clock diverges. Let $S_0=0$, and successively define

$$
U_j=\inf\{t\geq S_j:|\beta_t|=1\},\qquad S_{j+1}=\inf\{t\geq U_j:\beta_t=0\}.
$$

By [recurrence of one-dimensional Brownian motion](../../../../../../recurrence-of-one-dimensional-brownian-motion.md), all these times are finite almost surely. By the [Strong Markov property](../../../../../../strong-markov-property.md) at the returns $S_j$, the variables $D_j=(U_j-S_j)\wedge1$ are independent identically distributed, lie in $(0,1]$ almost surely, and have a strictly positive mean. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $\sum_jD_j=\infty$ almost surely. On $[S_j,U_j]$, $\beta_s\geq-1$, so

$$
\int_0^\infty e^{2\beta_s}ds\geq\sum_j\int_{S_j}^{U_j}e^{2\beta_s}ds\geq e^{-2}\sum_jD_j=\infty.
$$

The segments are disjoint, and their divergent duration also ensures they cannot accumulate at a finite time. This proves [Divergence of a driftless Brownian exponential clock](../../../../../../divergence-of-a-driftless-brownian-exponential-clock.md) and

$$
\boxed{[X]_\infty=[Y]_\infty=\infty\quad\text{almost surely}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
