<h1 id="question-3/d/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Choose the outward [orientation](../../../../../../../orientation-of-a-simplex.md) on the upper half of the [ellipsoid](../../../../../../../ellipsoid.md), giving counterclockwise [boundary orientation](../../../../../../../boundary-orientation.md) on $C$ as viewed from $z>0$. Parametrize the boundary [circle](../../../../../../../circle.md) by

$$
\mathbf c(t)=(\cos t,\sin t,0),\qquad0\leq t\leq2\pi.
$$

Then $\mathbf u(\mathbf c(t))=(-\sin t,\cos t,0)=\mathbf c'(t)$, so the [line integral](../../../../../../../line-integral.md) is

$$
\oint_C\mathbf u\cdot d\mathbf r
=\int_0^{2\pi}(\sin^2t+\cos^2t)\,dt=2\pi.
$$

For a direct [surface integral](../../../../../../../surface-integral.md), use the [parametrized surface](../../../../../../../parametrized-surface.md)

$$
\mathbf s(\varphi,t)=(\sin\varphi\cos t,\sin\varphi\sin t,\alpha\cos\varphi),
\qquad0\leq\varphi\leq\frac\pi2,\quad0\leq t\leq2\pi.
$$

Its outward [vector surface element](../../../../../../../vector-area-element.md) is supplied by the [cross product](../../../../../../../cross-product.md)

$$
\mathbf s_\varphi\times\mathbf s_t
=(\alpha\sin^2\varphi\cos t,\alpha\sin^2\varphi\sin t,
\sin\varphi\cos\varphi).
$$

Using the [curl](../../../../../../../curl.md) from [a](../../a.md),

$$
\iint_{S_\alpha}(\nabla\times\mathbf u)\cdot\mathbf n\,dS
=\int_0^{2\pi}\int_0^{\pi/2}2\sin\varphi\cos\varphi\,d\varphi\,dt
=\boxed{2\pi}.
$$

The two integrals agree for every $\alpha>0$, verifying the [Stokes theorem](../../../../../../../stokes-theorem.md). Only the vertical component of the [vector surface element](../../../../../../../vector-area-element.md) enters, which explains the absence of $\alpha$ in the answer.

## ↑ Ancestors (13)

1. [i](../i.md)
2. [d](../../d.md)
3. [Question 3](../../../question-3.md)
4. [Mathematics V resit](../../../../mathematics-v-resit-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
