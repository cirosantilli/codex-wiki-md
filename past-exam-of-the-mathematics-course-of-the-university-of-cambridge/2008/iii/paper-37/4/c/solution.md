<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Start the [planar Brownian motion](../../../../../../planar-brownian-motion.md) $X_t+iY_t$ at $-x$ and stop at $\tau=\inf\{t:X_t=0\}$. The complex exponential is holomorphic with nonzero derivative. By [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md), the process $e^{X_t+iY_t}$, run on its [conformal Brownian clock](../../../../../../conformal-brownian-clock.md)

$$
A_t=\int_0^{t\wedge\tau}e^{2X_s}\,ds,
$$

is planar [Brownian motion](../../../../../../brownian-motion-split.md) started at $\varepsilon=e^{-x}$, until its first exit from the unit disk. The clock is strictly increasing before $\tau$, and $A_\tau\leq\tau<\infty$ almost surely. It is legitimate to use the exponential although it is not globally injective: the Brownian coordinate brackets depend locally on the nonzero derivative, and the clock construction gives the stopped planar Brownian law. Before $\tau$, $|e^{X_t+iY_t}|<1$; at $\tau$ it equals one. Hence the disk exit time in the new clock is exactly $A_\tau$.

The continuous lifted argument of this path, starting from angle zero, is $Y_t$. Its total argument at exit is therefore $Y_\tau$, which has distribution $xC$ by part (b). If the winding count records only completed integer turns, it differs from $Y_\tau/(2\pi)$ by a remainder $R_\varepsilon$ with $|R_\varepsilon|\leq1$. If fractional turns are retained, that remainder is zero. In either convention, since $\log\varepsilon=-x$,

$$
\frac{\theta_\varepsilon}{\log\varepsilon}
=-\frac{Y_\tau}{2\pi x}-\frac{R_\varepsilon}{x}.
$$

The first term has distribution $-C/(2\pi)$ for every $x$, and the second tends to zero deterministically in absolute value as $x\to\infty$. Symmetry of the [Cauchy distribution](../../../../../../cauchy-distribution.md) removes the minus sign, so [Slutsky theorem](../../../../../../slutsky-theorem.md) gives the [small-radius Brownian winding law](../../../../../../small-radius-brownian-winding-law.md):

$$
\boxed{\frac{\theta_\varepsilon}{\log\varepsilon}\ \xrightarrow[\varepsilon\downarrow0]{d}\ \frac{C}{2\pi}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
