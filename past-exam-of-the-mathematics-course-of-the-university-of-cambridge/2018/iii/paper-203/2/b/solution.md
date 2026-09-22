<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Start the [Bessel process](../../../../../../bessel-process.md) at $x>0$ and let $\tau_0$ be its first hit of zero. Away from zero its [stochastic differential equation](../../../../../../stochastic-differential-equation.md) is

$$
dX_t=dW_t+\frac{\delta-1}{2X_t}\,dt.
$$

Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $f(x)=x^{2-\delta}$, localizing first to a compact interval in $(0,\infty)$. Its drift cancels:

$$
\frac12f''(x)+\frac{\delta-1}{2x}f'(x)
=\frac{(2-\delta)(1-\delta)}2x^{-\delta}
+\frac{(\delta-1)(2-\delta)}2x^{-\delta}=0.
$$

Thus the [Bessel power local martingale](../../../../../../bessel-power-local-martingale.md) satisfies

$$
\boxed{d(X_t^{2-\delta})=(2-\delta)X_t^{1-\delta}\,dW_t\qquad(t<\tau_0).}
$$

For $\delta=2$, this power is simply the constant one. For $\delta>2$, it is a [continuous local martingale](../../../../../../continuous-local-martingale.md) for all time, as zero is inaccessible.

Here is a proof of that inaccessibility and of the stronger minimum assertion. For $0<r<x<R$, stop the power at $\tau_r\wedge\tau_R$. The stopped process is bounded, so the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
\mathbb P_x(\tau_r<\tau_R)
=\frac{x^{2-\delta}-R^{2-\delta}}{r^{2-\delta}-R^{2-\delta}}.
$$

Exit from the bounded interval occurs almost surely. Taking $r\downarrow0$ with $R$ fixed shows that zero cannot be hit before $R$, hence cannot be hit in finite time. Taking $R\to\infty$ instead gives

$$
\mathbb P_x(\tau_r<\infty)=\left(\frac r x\right)^{\delta-2}.
$$

If the all-time infimum were zero, every level $r>0$ below $x$ would be hit, by [continuity](../../../../../../continuous-function.md). Letting $r\downarrow0$ proves the [all-time minimum of a transient Bessel process](../../../../../../all-time-minimum-of-a-transient-bessel-process.md) assertion:

$$
\boxed{\delta>2,\ X_0>0\quad\Longrightarrow\quad\inf_{t\geq0}X_t>0\quad\text{almost surely}.}
$$

The first claim in the printed question needs a qualification when $\delta<2$: it holds before the first hit of zero, or for the process stopped there, rather than for the usual reflecting continuation. For example, at $\delta=1$ the proposed power is $X$ itself, a [Reflected Brownian motion](../../../../../../reflected-brownian-motion.md); the [Tanaka formula](../../../../../../tanaka-s-formula.md) contains a nonzero [local time of a semimartingale](../../../../../../local-time-of-a-semimartingale.md) term, so it is not a [local martingale](../../../../../../local-martingale.md) after reflection. A positive starting point is also needed for the negative power when $\delta>2$; an entrance process started at zero would give an infinite value at time zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
