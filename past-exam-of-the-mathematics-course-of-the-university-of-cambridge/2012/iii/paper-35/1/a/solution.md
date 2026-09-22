<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [half-plane-capacity parameterization](../../../../../../half-plane-capacity-parameterization.md) in which $g_t(z)=z+2t/z+O(z^{-2})$ at infinity. The [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) is

$$
\boxed{\partial_tg_t(z)=\frac{2}{g_t(z)-W_t},\qquad g_0(z)=z,\qquad W_t=\sqrt\kappa\,\beta_t.}
$$

It holds up to the [Loewner swallowing time](../../../../../../interior-point-swallowing-time-for-a-loewner-chain.md) of $z$. Although $\beta$ is nowhere differentiable, it is continuous: the equation for $g$ is an ordinary integral equation with a continuous time-dependent coefficient away from its pole.

For $x\in\mathbb R\setminus\{0\}$, the same real-valued equation has a unique solution until $g_t(x)-W_t$ first reaches zero. Its solution agrees with the boundary value of the [conformal map](../../../../../../conformal-map.md) from the unswallowed side. One can also obtain it by [Schwarz reflection](../../../../../../schwarz-reflection-principle.md) across an unswallowed real interval. Thus

$$
\boxed{T(x)=\inf\{t:g_t(x)=W_t\}}
$$

is the [boundary-point swallowing time for a Loewner chain](../../../../../../boundary-point-swallowing-time-for-a-loewner-chain.md); it can be infinite. The collision definition agrees with membership in the closed hull. The initial point has $T(0)=0$. Swallowing a real point is not the same as visiting it: a curve can cut off an entire real interval in one step.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
