<h1 id="question-3/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Choose the outward [unit normal vector](../../../../../../../unit-normal.md) on the upper [hemisphere](../../../../../../../hemisphere.md). The [curl](../../../../../../../curl.md) of $\mathbf F=(4y,x,2z)$ is

$$
\nabla\times\mathbf F=(0,0,1-4)=(0,0,-3).
$$

In [spherical polar coordinates](../../../../../../../spherical-coordinate-system.md), put

$$
\mathbf s(\varphi,\theta)
=a(\sin\varphi\cos\theta,\sin\varphi\sin\theta,\cos\varphi),
\qquad0\leq\varphi\leq\frac\pi2,\quad0\leq\theta\leq2\pi.
$$

Here $n_z=\cos\varphi$ and $dS=a^2\sin\varphi\,d\varphi\,d\theta$. The [surface integral](../../../../../../../surface-integral.md) is therefore

$$
\iint_\Sigma(\nabla\times\mathbf F)\cdot\mathbf n\,dS
=-3a^2\int_0^{2\pi}\int_0^{\pi/2}\cos\varphi\sin\varphi\,d\varphi\,d\theta
=\boxed{-3\pi a^2}.
$$

The compatible [boundary orientation](../../../../../../../boundary-orientation.md) follows increasing $t$ in $\mathbf r(t)=(a\cos t,a\sin t,0)$, $0\leq t\leq2\pi$. On this [circle](../../../../../../../circle.md),

$$
\mathbf F(\mathbf r(t))=(4a\sin t,a\cos t,0),\qquad
\mathbf r'(t)=(-a\sin t,a\cos t,0).
$$

Thus the [line integral](../../../../../../../line-integral.md) is

$$
\oint_{\partial\Sigma}\mathbf F\cdot d\mathbf r
=a^2\int_0^{2\pi}(-4\sin^2t+\cos^2t)\,dt
=\boxed{-3\pi a^2},
$$

which agrees with the [surface integral](../../../../../../../surface-integral.md) as required by the [Stokes theorem](../../../../../../../stokes-theorem.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
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
