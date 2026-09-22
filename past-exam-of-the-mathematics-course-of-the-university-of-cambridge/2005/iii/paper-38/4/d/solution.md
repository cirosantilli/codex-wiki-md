<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $t>1$, $B_{t^2}$ is not measurable with respect to the original Brownian filtration $\mathcal F_t$: its conditional variance is $t^2-t>0$. Thus it is not even adapted on the full half-line. It also fails the [martingale](../../../../../../martingale-split.md) condition before time one. With $s=1/4$, $t=3/4$,

$$
\mathbb E[B_{t^2}\mid\mathcal F_s]=B_s\ne B_{s^2}=M_s.
$$

The appropriate filtration is

$$
\boxed{\mathcal G_t=\mathcal F_{t^2}}.
$$

Brownian [independent increments](../../../../../../independent-increments.md) make $M_t=B_{t^2}$ a continuous $\mathcal G_t$-martingale, with [quadratic variation](../../../../../../quadratic-variation.md) $[M]_t=t^2$. Define the [stochastic integral](../../../../../../stochastic-integral.md)

$$
W_t=\int_0^t\frac{1}{\sqrt{2s}}\,dM_s.
$$

The value of the integrand at zero is immaterial; it is square-integrable against the bracket because $\int_0^t(2s)^{-1}\,d(s^2)=t$. Consequently $[W]_t=t$, and the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) makes $W$ a $\mathcal G_t$-Brownian motion. Associativity of [stochastic integrals](../../../../../../stochastic-integral.md) gives the [Brownian motion under a quadratic time change](../../../../../../brownian-motion-under-a-quadratic-time-change.md) representation

$$
\boxed{M_t=\int_0^t\sqrt{2s}\,dW_s,\qquad f(s)=\sqrt{2s}}.
$$

The function $f$ is continuous at zero. One can first verify the inverse-integrand identity on $[\varepsilon,t]$ and then let $\varepsilon\downarrow0$ using the [Itô isometry](../../../../../../ito-isometry.md), since $\mathbb EM_\varepsilon^2=\varepsilon^2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
