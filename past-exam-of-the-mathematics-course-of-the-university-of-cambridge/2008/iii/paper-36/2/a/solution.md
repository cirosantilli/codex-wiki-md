<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For chordal [SLE](../../../../../../schramm-loewner-evolution.md) with parameter $\kappa$, the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) $\gamma$ starts at zero and is parametrized by [half-plane capacity](../../../../../../half-plane-capacity.md) $2t$. Let $D_t$ be the unbounded component of $\mathbb H\setminus\gamma[0,t]$, and let $K_t=\mathbb H\setminus D_t$ be its filled [compact H-hull](../../../../../../compact-h-hull.md). When the trace is not simple, the hull includes the regions it disconnects from infinity. The associated [mapping-out functions of compact H-hulls](../../../../../../mapping-out-function-of-a-compact-h-hull.md) have expansion

$$
g_t(z)=z+\frac{2t}{z}+O(z^{-2})
$$

and satisfy the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md)

$$
\boxed{\partial_tg_t(z)=\frac2{g_t(z)-\xi_t},\qquad
g_0(z)=z,\qquad\xi_t=\sqrt\kappa\,B_t,}
$$

where $B$ is standard real [Brownian motion](../../../../../../brownian-motion-split.md). The equation is solved until $z$ is swallowed by the hull. The [Loewner transform](../../../../../../loewner-driving-function.md) $\xi$ records the real boundary point at which the mapped hull grows; its relation to the trace is

$$
\gamma_t=\lim_{y\downarrow0}g_t^{-1}(\xi_t+iy).
$$

Equivalently the tip maps to $\xi_t$ in the appropriate boundary prime-end sense. Thus the flow encodes the surviving domains, the transform drives that flow, and the trace generates its hulls. For $\kappa=0$, the driver is identically zero, $g_t(z)=\sqrt{z^2+4t}$ with the branch asymptotic to $z$, and $\gamma_t=2i\sqrt t$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
