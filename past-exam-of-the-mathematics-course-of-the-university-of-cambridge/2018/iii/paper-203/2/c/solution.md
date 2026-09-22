<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\kappa>0$ and $x>0$, before the boundary point is swallowed, put $X_t=(g_t(x)-U_t)/\sqrt\kappa$. The [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) and $dU_t=\sqrt\kappa\,dB_t$ give

$$
dX_t=\frac{2}{\kappa X_t}\,dt-dB_t.
$$

Since $-B$ is again a standard [Brownian motion](../../../../../../brownian-motion-split.md), this is the [Boundary-point Bessel flow for SLE](../../../../../../boundary-point-bessel-flow-for-sle.md) with

$$
\boxed{\delta=1+\frac4\kappa.}
$$

For $x<0$, it is $-X_t$ that is the nonnegative [Bessel process](../../../../../../bessel-process.md), with the same dimension; the formula without this sign convention is a signed Bessel flow.

When $0<\kappa\leq4$, one has $\delta\geq2$, and the [Hitting-zero classification for a Bessel process](../../../../../../hitting-zero-classification-for-a-bessel-process.md) says that $X_t$ never reaches zero. The borderline $\delta=2$ uses the [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md) $\log x$: for $0<r<x<R$,

$$
\mathbb P_x(\tau_r<\tau_R)=\frac{\log R-\log x}{\log R-\log r}\longrightarrow0\quad(r\downarrow0).
$$

Thus the critical case also cannot hit zero in finite time, though its all-time infimum is zero.

Apply the non-swallowing assertion simultaneously to all nonzero rational boundary points. The order-preserving real Loewner flow then keeps every compact real interval away from the origin in the surviving boundary. A boundary contact away from the starting point would cut off a nonempty real interval, swallowing a rational point, so the trace avoids $\mathbb R\setminus\{0\}$.

The same argument can be applied to the future after every rational time, using the [Conformal Markov property of SLE](../../../../../../conformal-markov-property-of-sle.md). If the trace revisited an earlier point, choose a rational time strictly between the two visits. In the domain with that initial segment removed, the later visit would be a contact with an old boundary point away from the current growing tip. Under the mapping-out map, such a contact cuts off a real interval and contradicts the preceding non-swallowing result. This is the usual [crosscut](../../../../../../crosscut.md) argument converting boundary non-swallowing into absence of self-intersections. Taking the countable intersection over rational restart times proves

$$
\boxed{\operatorname{SLE}_\kappa\text{ is simple for }0<\kappa\leq4.}
$$

For $\kappa=0$, the equation is deterministic and gives the simple slit $(0,2i\sqrt t]$. The division by $\sqrt\kappa$ is unnecessary in that case.

## ↑ Ancestors (11)

1. [C](../c.md)
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
