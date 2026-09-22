<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The clock $A_t=\int_0^te^{2\beta_s}ds$ is continuous, strictly increasing and unbounded. Define $\tau_r=\inf\{t:A_t\geq r\}$. Part (a), with the initial vector retained, proves that

$$
\boxed{\mathcal B_r=Z_{\tau_r}\text{ is planar Brownian motion started at }(1,0)\text{ in }\mathcal F_{\tau_r}.}
$$

Every finite $r$ has finite $\tau_r$, and $|\mathcal B_r|=e^{\beta_{\tau_r}}>0$. On the common event where the clock is a continuous bijection of $[0,\infty)$, this holds simultaneously for all times. Thus the origin is a [polar point for planar Brownian motion](../../../../../../polar-point-for-planar-brownian-motion.md) started at $(1,0)$:

$$
\boxed{\mathbb P(\mathcal B_r\ne0\text{ for all }r\geq0)=1.}
$$

To prove unbounded-time visits near zero, let $t_n=\inf\{t\geq n:\beta_t=-n\}$. Brownian recurrence makes each $t_n$ finite almost surely, and $t_n\geq n\to\infty$. Set $r_n=A_{t_n}$. Since $A_t\to\infty$, $r_n\to\infty$, while

$$
|\mathcal B_{r_n}|=|Z_{t_n}|=e^{-n}\longrightarrow0.
$$

Consequently

$$
\boxed{\liminf_{r\to\infty}|\mathcal B_r|=0\quad\text{almost surely}.}
$$

For every fixed neighbourhood of zero there are visits at arbitrarily large times. Since $\mathcal B$ has the law of planar [Brownian motion](../../../../../../brownian-motion-split.md) with this initial value, both conclusions hold for that Brownian law. This [complex exponential construction of planar Brownian motion](../../../../../../complex-exponential-construction-of-planar-brownian-motion.md) proves the two properties together without confusing recurrence near a point with hitting the point.

## ↑ Ancestors (11)

1. [C](../c.md)
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
