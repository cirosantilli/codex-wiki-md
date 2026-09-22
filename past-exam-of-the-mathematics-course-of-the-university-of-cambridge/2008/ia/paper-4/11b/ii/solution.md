<h1 id="11b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $D=(d/dt)_S$, $D'=(d/dt)_{S'}$, and $\mathbf v'=D'\mathbf r$. By the [rotating-frame derivative formula](../../../../../../rotating-frame-derivative-formula.md), $D\mathbf r=\mathbf v'+\boldsymbol\omega\times\mathbf r$. Apply the [product rule](../../../../../../product-rule.md) for the [cross product](../../../../../../cross-product.md) and the same [rotating-frame derivative formula](../../../../../../rotating-frame-derivative-formula.md) again:

$$
D^2\mathbf r=D\mathbf v'+(D\boldsymbol\omega)\times\mathbf r+\boldsymbol\omega\times D\mathbf r.
$$

We have $D\mathbf v'=D'\mathbf v'+\boldsymbol\omega\times\mathbf v'$ and $D\boldsymbol\omega=D'\boldsymbol\omega$, since $\boldsymbol\omega\times\boldsymbol\omega=0$. Therefore

$$
\boxed{D^2\mathbf r=D'^2\mathbf r+2\boldsymbol\omega\times D'\mathbf r+(D'\boldsymbol\omega)\times\mathbf r+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r).}
$$

Rearranging this identity into an [equation of motion in a rotating frame](../../../../../../equation-of-motion-in-a-rotating-frame.md) produces the apparent [Coriolis acceleration](../../../../../../coriolis-acceleration.md), [Euler acceleration](../../../../../../euler-acceleration.md) and [centrifugal acceleration](../../../../../../centrifugal-acceleration.md), with signs opposite to their corresponding terms on the right of this inertial [acceleration](../../../../../../acceleration.md) identity. No translational term is needed because the two origins coincide.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11B](../../11b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
