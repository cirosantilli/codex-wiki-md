<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $\Delta M=M_1-M_0$ and retain only terms first order in $\mu/M_0$ and $\rho/M_0$. The outgoing [event horizon](../../../../../../event-horizon.md) equation expands to

$$
4M_0\dot\rho=\rho-2\mu,
\qquad \dot\rho-\kappa_0\rho=-\frac{\mu}{2M_0},
\qquad \kappa_0=\frac1{4M_0}.
$$

Here $\kappa_0$ is the initial [Schwarzschild surface gravity](../../../../../../schwarzschild-surface-gravity.md). The [integrating factor](../../../../../../integrating-factor.md) $e^{-\kappa_0v}$ gives $d(e^{-\kappa_0v}\rho)/dv=-e^{-\kappa_0v}\mu/(2M_0)$. Future stationarity imposes $\rho=2\Delta M$ for $v>v_0$ and removes the growing homogeneous solution. Integrating from $v$ to infinity yields the [teleological response of a Vaidya event horizon](../../../../../../teleological-response-of-a-vaidya-event-horizon.md):

$$
\boxed{\rho(v)=\frac1{2M_0}\int_v^\infty e^{-\kappa_0(s-v)}\mu(s)\,ds.}
$$

The integral is finite because $\mu$ is bounded. Integrating by parts also gives

$$
\rho(v)=2\mu(v)+2\int_v^\infty e^{-\kappa_0(s-v)}\dot\mu(s)\,ds.
$$

For $v>v_0$, this reduces to $2\Delta M$. For $v<0$, the first form becomes

$$
\rho(v)=C e^{\kappa_0v},\qquad C=\frac1{2M_0}\int_0^\infty e^{-\kappa_0s}\mu(s)\,ds.
$$

Consequently **$r_H\to2M_0$ as $v\to-\infty$**. The positive constant $C$ shows that this [event horizon](../../../../../../event-horizon.md) is already expanding in the initially vacuum region. For monotone accretion, $\rho-2\mu\geq0$, so it lies outside the instantaneous [apparent horizon](../../../../../../apparent-horizon.md) to first order. All displayed radius corrections are understood up to $O((\Delta M)^2/M_0)$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
