<h1 id="question-3/b/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Use the outward [orientation](../../../../../../../orientation-of-a-simplex.md) on the unit [hemisphere](../../../../../../../hemisphere.md) and counterclockwise [boundary orientation](../../../../../../../boundary-orientation.md) on the unit [circle](../../../../../../../circle.md). With $\mathbf r(t)=(\cos t,\sin t,0)$ and $f=x=\cos t$, the vector [line integral](../../../../../../../line-integral.md) is

$$
\begin{aligned}
\oint_{\partial\Sigma}f\,d\mathbf r
&=\int_0^{2\pi}(-\cos t\sin t,\cos^2t,0)\,dt\\
&=\boxed{(0,\pi,0)}.
\end{aligned}
$$

For the [surface integral](../../../../../../../surface-integral.md), $\nabla f=\mathbf i$ and the outward [unit normal vector](../../../../../../../unit-normal.md) is $\mathbf n=(x,y,z)$, since the radius is one. The [cross product](../../../../../../../cross-product.md) is

$$
\mathbf n\times\nabla f=(0,z,-y).
$$

The [integral](../../../../../../../integral-split.md) of $y$ is zero by [reflection symmetry](../../../../../../../reflection-symmetry.md). Using the same [spherical polar coordinates](../../../../../../../spherical-coordinate-system.md) as in [ii](../../a/ii.md), with $a=1$, the other component is

$$
\iint_\Sigma z\,dS
=\int_0^{2\pi}\int_0^{\pi/2}\cos\varphi\sin\varphi\,d\varphi\,d\theta
=\pi.
$$

Hence

$$
\boxed{\iint_\Sigma(\mathbf n\times\nabla f)\,dS=(0,\pi,0)},
$$

verifying the [vector-valued Stokes identity](../../../../../../../vector-valued-stokes-identity.md) directly, component by component. The wedge symbol in the paper denotes the [cross product](../../../../../../../cross-product.md) here.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [b](../../b.md)
3. [Question 3](../../../question-3.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
