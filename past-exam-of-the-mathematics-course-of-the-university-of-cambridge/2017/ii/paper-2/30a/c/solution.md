<h1 id="30a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the unforced undamped pendulum, the upper homoclinic separatrix has energy $E=p^2/2-\cos\theta=1$ and $p_0(\theta)=2\cos(\theta/2)$ for $-\pi\leq\theta\leq\pi$. With forcing and damping,

$$
\dot E=Fp-kp^2.
$$

The first-order energy change along this separatrix is

$$
\Delta E=F\int_{-\pi}^{\pi}d\theta-k\int_{-\pi}^{\pi}p_0(\theta)\,d\theta=2\pi F-8k.
$$

The zero of this first-order stable/unstable-manifold splitting is simple in $F$. Smooth dependence of the saddle manifolds and the implicit function theorem therefore give a nearby homoclinic branch with

$$
\boxed{F_h(k)=\frac4\pi k+O(k^2).}
$$

The asymptotic formula is the leading-order stable/unstable-manifold balance. On a lower homoclinic orbit, $p\leq0$ and the lifted angle decreases by $2\pi$, so the exact integrated energy balance would be

$$
0=-2\pi F-k\int_{-\infty}^{\infty}p^2\,dt<0
$$

when $F>0$. Hence **no lower homoclinic orbit exists for positive forcing**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30A](../../30a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
