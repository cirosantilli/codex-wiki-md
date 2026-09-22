<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Bingham plastic](../../../../../../bingham-plastic.md) is a [yield-stress fluid](../../../../../../yield-stress-fluid.md), and hence a [non-Newtonian fluid](../../../../../../non-newtonian-fluid.md). It is also an instantaneous generalized-Newtonian model after yielding. It cannot describe memory-dependent [viscoelasticity](../../../../../../viscoelasticity.md), including stress relaxation, elastic recoil, and time-dependent normal-stress effects.

For scalar shear stress $\tau$ and shear rate $\dot\gamma$, its complete ideal constitutive law is

$$
\begin{cases}
\dot\gamma=0, & |\tau|\leq\sigma_y,\\
\tau=\sigma_y\operatorname{sgn}(\dot\gamma)+\eta\dot\gamma,
& |\tau|>\sigma_y.
\end{cases}
$$

Equivalently, in yielded material,

$$
\boxed{\dot\gamma=\frac{|\tau|-\sigma_y}{\eta}\operatorname{sgn}\tau.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 352](../../../paper-352-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
