<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $L_r=\theta_{T_r}$. The hitting times $T_r$ are finite [almost surely](../../../../../../almost-sure-convergence.md) by [recurrence of planar Brownian motion](../../../../../../recurrence-of-planar-brownian-motion.md), and increase with $r$. At $T_r$, the position is $e^{-r}e^{iL_r}$. By the [Strong Markov property](../../../../../../strong-markov-property.md), [Brownian scaling](../../../../../../brownian-scaling.md), and [rotational invariance of planar Brownian motion](../../../../../../rotational-invariance-of-planar-brownian-motion.md), the future process

$$
\widehat B_u=e^r e^{-iL_r}B_{T_r+e^{-2r}u}
$$

is a standard [planar Brownian motion](../../../../../../planar-brownian-motion.md) started at $1$, independent of $\mathcal F_{T_r}$. The random rotation does not change its conditional law, since that law is rotationally invariant.

The first time this rescaled process reaches radius $e^{-h}$ corresponds to the original time $T_{r+h}$. Its continuous argument starts at zero and equals the increment of the original winding angle. Hence

$$
\boxed{L_{r+h}-L_r\ \text{is independent of }\mathcal F_{T_r}
\text{ and has the law of }L_h.}
$$

For any ordered finite collection of levels, apply this assertion successively. Earlier winding values are measurable at the current hitting time, so all increments are independent and their laws depend only on the level differences. This proves the [Lévy process](../../../../../../levy-process.md) property of [winding at logarithmic radial passage levels](../../../../../../winding-at-logarithmic-radial-passage-levels.md).

One can also verify stochastic continuity and identify this process. The logarithmic-radius and argument martingales have the common clock

$$
H_t=\int_0^t|B_s|^{-2}\,ds.
$$

The same [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) calculation as in part (a), applied locally to the logarithm and joined along the continuous argument, gives independent [Brownian motions](../../../../../../brownian-motion-split.md) $U,V$ such that $\log R_t=U_{H_t}$ and $\theta_t=V_{H_t}$. This clock diverges: if it had a finite limit, convergence of martingales with finite total [quadratic variation](../../../../../../quadratic-variation.md) would make $\log R_t$ converge to a finite value, forcing the clock integral itself to diverge.

Thus, with $\eta_r=\inf\{u:U_u=-r\}$, we have $L_r=V_{\eta_r}$. The [Brownian first-passage Laplace transform](../../../../../../brownian-first-passage-laplace-transform.md) is $\mathbb E e^{-q\eta_r}=e^{-r\sqrt{2q}}$. It follows either from the [Exponential martingale for Brownian motion](../../../../../../exponential-martingale-for-brownian-motion.md) stopped at $\eta_r\wedge n$, or from the one-dimensional exit equation. Conditioning on the independent process $U$ gives

$$
\boxed{\mathbb E e^{i\lambda L_r}=\mathbb E e^{-\lambda^2\eta_r/2}=e^{-r|\lambda|}.}
$$

So this is a symmetric [Cauchy process](../../../../../../cauchy-process.md), with level parameter $r$. The formula implies stochastic continuity at zero and, by stationary increments, everywhere. Under the usual definition requiring [càdlàg](../../../../../../cadlag.md) paths, use the right-continuous passage clock $\eta_r^+=\inf\{u:U_u<-r\}$. It agrees with $\eta_r$ for each fixed level [almost surely](../../../../../../almost-sure-convergence.md), and $V_{\eta_r^+}$ is the [càdlàg](../../../../../../cadlag.md) modification. This distinction concerns simultaneous passage levels and does not alter any increment law.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
