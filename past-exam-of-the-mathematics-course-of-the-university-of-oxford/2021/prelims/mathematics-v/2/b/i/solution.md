<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Parametrize the [surface of revolution](../../../../../../../surface-of-revolution.md) by

$$
\mathbf X(t,\theta)=(\cos t\cos\theta,\cos t\sin\theta,f(t)),\quad
-\pi/2\leq t\leq\pi/2,\quad0\leq\theta<2\pi.
$$

An oriented [vector surface area element](../../../../../../../vector-surface-area-element.md) is

$$
\mathbf X_\theta\times\mathbf X_t
=(\cos t f'(t)\cos\theta,\cos t f'(t)\sin\theta,\sin t\cos t).
$$

Use the [vector field](../../../../../../../vector-field.md) $\mathbf F=(x/2,y/2,0)$, whose [divergence](../../../../../../../divergence.md) is one. If this [parametrization](../../../../../../../parametric-equation.md) has the outward orientation on an enclosing surface, the [divergence theorem](../../../../../../../divergence-theorem.md) gives

$$
\boxed{V=\pi\int_{-\pi/2}^{\pi/2}\cos^2t\,f'(t)\,dt
=\pi\int_{-\pi/2}^{\pi/2}f(t)\sin2t\,dt.}
$$

The second equality is [integration by parts](../../../../../../../integration-by-parts.md), using the endpoint values. For example this outward convention applies when the positive-$t$ branch lies above the negative-$t$ branch, $f(t)>f(-t)$ for $0<t<\pi/2$.

The stated $C^1$ regularity and endpoint conditions alone do not guarantee an embedded enclosing surface: branches can cross or coincide. Without an appropriate orientation assumption the [flux](../../../../../../../flux.md) formula is an algebraic signed [volume](../../../../../../../volume.md). If “inside” is defined as the region between the two graph branches for each radius, its nonnegative geometric [volume](../../../../../../../volume.md) is instead

$$
V=2\pi\int_0^{\pi/2}\sin t\cos t\,|f(t)-f(-t)|\,dt.
$$

This explicitly handles a reversal or change in the order of the two branches.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
