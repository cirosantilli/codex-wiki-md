<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The finite-$p$ assertion needs the zero-divergence hypothesis from the preceding part, which is not repeated in this part's printed hypotheses. The [norm](../../../../../../norm.md) is on $\mathbb R^3_x\times\mathbb R^3_v$, and finite conservation requires $f_0$ to belong to the corresponding [Lp space](../../../../../../lp-space.md) in addition to its smoothness.

Writing $\Phi_t$ for the [characteristic flow map](../../../../../../characteristic-flow-map.md), the general solution is $f_t=f_0\circ\Phi_t^{-1}$. A [change of variables](../../../../../../change-of-variables-formula.md) gives

$$
\|f_t\|_p^p=\int_{\mathbb R^6}|f_0(z)|^pJ(t,z)\,dz.
$$

Thus the [Lp conservation for incompressible transport](../../../../../../lp-conservation-for-incompressible-transport.md) is

$$
\boxed{\nabla_v\cdot F=0\quad\Longrightarrow\quad\|f_t\|_p=\|f_0\|_p,\quad1\leq p<\infty}.
$$

Without that condition the requested conclusion is false: the force in part (c), together with any nonzero smooth integrable initial datum given by a [Gaussian function](../../../../../../gaussian-function.md), gives $\|f_t\|_p=e^{3t/p}\|f_0\|_p$. The [essential supremum](../../../../../../essential-supremum.md) is still conserved by a complete invertible flow, because composition does not change the range of values.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
