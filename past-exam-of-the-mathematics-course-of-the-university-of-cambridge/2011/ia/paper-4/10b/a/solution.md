<h1 id="10b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At $P$, use the local right-handed basis $\mathbf e_E,\mathbf e_N,\mathbf e_U$ pointing east, north and vertically outward. The Earth's rotation vector has components

$$
\boldsymbol\omega=\omega(\sin\theta\,\mathbf e_N+\cos\theta\,\mathbf e_U),\qquad
\mathbf r=R\mathbf e_U.
$$

Initially $\dot{\mathbf r}=0$ in the [rotating reference frame](../../../../../../rotating-reference-frame.md), so the [Coriolis acceleration](../../../../../../coriolis-acceleration.md) is zero. Evaluating the [centrifugal acceleration](../../../../../../centrifugal-acceleration.md) gives

$$
-\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf r)
=\omega^2R(\sin^2\theta\,\mathbf e_U-\sin\theta\cos\theta\,\mathbf e_N).
$$

The [gravitational acceleration](../../../../../../gravitational-acceleration.md) is $-g\mathbf e_U$. Hence

$$
\ddot{\mathbf r}(0)
=-(g-\omega^2R\sin^2\theta)\mathbf e_U
-\omega^2R\sin\theta\cos\theta\,\mathbf e_N.
$$

The small angle $\delta$ from the downward vertical therefore satisfies

$$
\tan\delta=\frac{\omega^2R|\sin\theta\cos\theta|}{g-\omega^2R\sin^2\theta},\qquad
\boxed{\delta\simeq\frac{\omega^2R}{g}|\sin\theta\cos\theta|.}
$$

For the northern hemisphere, $0\leq\theta\leq\pi/2$, this is the printed expression without absolute values. More generally, the printed signed meridional expression specifies the direction of the tilt; an unsigned angle uses its absolute value. The horizontal component is toward the equator and vanishes at both poles and at the equator.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
