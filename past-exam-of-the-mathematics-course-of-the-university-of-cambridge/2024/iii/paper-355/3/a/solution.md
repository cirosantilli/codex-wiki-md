<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the unit normal $\mathbf n$ point from the fluid toward the free surface, let $\mathbf t$ lie along the surface, and write the swimmer direction as

$$
\mathbf p=\cos\theta\,\mathbf t+\sin\theta\,\mathbf n.
$$

Reflecting the swimmer position across the plane and reflecting its orientation to

$$
\mathbf p^*=\cos\theta\,\mathbf t-\sin\theta\,\mathbf n
$$

constructs the [free-surface image of a force dipole](../../../../../../free-surface-image-of-a-force-dipole.md). At the surface the two dipoles have equal tangential velocity and opposite normal velocity. Their sum therefore satisfies the [no-penetration boundary condition](../../../../../../no-penetration-boundary-condition.md); tangential velocity is even across the plane and normal velocity is odd, so the tangential traction vanishes and the [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) is also satisfied.

The vector from the image to the swimmer is $\mathbf r=-2h\mathbf n$, for which $(\mathbf p^*\mathbin\cdot\mathbf r)^2=4h^2\sin^2\theta$. Evaluating the image [force-dipole flow](../../../../../../force-dipole-flow.md) at the swimmer gives

$$
\boxed{
\mathbf U_{\rm surf}
=\frac{\mathcal P}{32\pi\mu h^2}
\left(1-3\sin^2\theta\right)\mathbf n
}.
$$

There is no tangential image velocity at the swimmer in this point-dipole approximation. With the convention that $\mathcal P>0$ is an extensile [pusher microswimmer](../../../../../../pusher-microswimmer.md), a nearly parallel pusher is attracted toward the surface, whereas a nearly parallel contractile [puller microswimmer](../../../../../../puller-microswimmer.md) is repelled. For $|\sin\theta|>1/\sqrt3$ the normal drift reverses because the image samples the axial rather than equatorial part of the dipolar flow.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
