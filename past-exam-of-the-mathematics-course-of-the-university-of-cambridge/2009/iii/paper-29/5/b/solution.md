<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $H$ is continuous, strictly increasing and unbounded, $J_t=\inf\{s>0:H_s>t\}$ is its continuous inverse: $H_{J_t}=t$, $J_{H_s}=s$ and $J_0=0$. These inverse times are [stopping times](../../../../../../stopping-time.md). Put $X_t=Y_{J_t}$, which is continuous and strictly positive and is adapted to the inverse-clock filtration $\mathcal G_t=\mathcal F_{J_t}$.

Evaluate the identity from part (a) at $J_t$. The Lebesgue-Stieltjes change of variable $r=H_s$ gives

$$
\int_0^{J_t}\frac1{Y_s}\,dH_s=\int_0^{H_{J_t}}\frac1{Y_{J_r}}dr=\int_0^t\frac1{X_r}dr.
$$

Therefore

$$
\boxed{X_t=1+\beta_t+\int_0^t\frac1{X_s}ds,\qquad dX_t=d\beta_t+\frac1{X_t}dt.}
$$

The process $\beta$ is [Brownian motion](../../../../../../brownian-motion-split.md) in this same filtration by the construction in part (a). The drift integral is finite on each compact interval because the positive continuous process $X$ has a positive minimum there. This is the dimension-three case of the [Exponential Brownian-to-Bessel time change](../../../../../../exponential-brownian-to-bessel-time-change.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
