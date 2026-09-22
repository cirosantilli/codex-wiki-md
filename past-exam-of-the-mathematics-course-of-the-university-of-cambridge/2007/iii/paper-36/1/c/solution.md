<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First justify that the logarithm is defined at all times from one onward. For planar [Brownian motion](../../../../../../brownian-motion-split.md) started at $z\ne0$, stop on exiting the annulus $\varepsilon<|x|<R$, where $\varepsilon<|z|<R$. This exit time $\rho$ is finite almost surely: the stopped identity $|B_t|^2-2t$ gives $\mathbb E(t\wedge\rho)\le R^2/2$. The function $f(x)=\log|x|$ is harmonic on the annulus, so its [stopped process](../../../../../../stopped-process.md) is a bounded [martingale](../../../../../../martingale-split.md). Optional stopping gives

$$
\mathbb P_z(\text{hit }\varepsilon\text{ before }R)=\frac{\log R-\log|z|}{\log R-\log\varepsilon}\longrightarrow0.
$$

Hitting zero before the outer circle would require hitting every inner circle first. It therefore has probability zero. Taking a countable sequence of outer radii tending to infinity proves that [planar Brownian motion avoids a fixed point](../../../../../../planar-brownian-motion-avoids-a-fixed-point.md). Since $B_1$ has a density and is nonzero almost surely, condition on $\mathcal F_1$ to apply this result to the future path.

For $x\ne0$, $\nabla f(x)=x/|x|^2$ and $\Delta f(x)=0$ in two dimensions. The [Itô formula](../../../../../../ito-s-lemma.md) on annuli therefore gives

$$
\boxed{X_t=X_1+\int_1^t\frac{B_s}{|B_s|^2}\cdot dB_s\qquad(t\ge1).}
$$

To localize explicitly, let $\tau_n=\inf\{t\ge1:|B_t|\notin(1/n,n)\}$. These [stopping times](../../../../../../stopping-time.md) increase to infinity almost surely: on each compact time interval the continuous path has a finite maximum and, by point avoidance, a positive minimum radius. Up to $\tau_n$, the stochastic integrand has norm at most $n$. Its stopped integral is square-integrable on every finite horizon. The initial value $\log|B_1|$ is integrable, as follows from the Rayleigh-density calculation in part d. Hence $X^{\tau_n}$ is a true [martingale](../../../../../../martingale-split.md) from time one and **$X$ is a [local martingale](../../../../../../local-martingale.md)**. This also gives its [quadratic variation](../../../../../../quadratic-variation.md) from time one as $\int_1^t|B_s|^{-2}\,ds$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
