<h1 id="39b/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\tau$ be the time at which a right-running [characteristic curve](../../../../../../../characteristic-curve.md) leaves the piston. The boundary velocity and the characteristic it emits are

$$
u=a\omega\cos(\omega\tau),
\qquad
x=a\sin(\omega\tau)+c_0(t-\tau).
$$

With

$$
\phi=\omega\left(t-\frac{x}{c_0}\right),
\qquad
\theta=\omega\tau,
\qquad
\epsilon=\frac{a\omega}{c_0}<1,
$$

these relations become

$$
\boxed{\phi=\theta-\epsilon\sin\theta,
\qquad U(\phi)=a\omega\cos\theta}.
$$

Because $d\phi/d\theta=1-\epsilon\cos\theta>0$ and $\phi(\theta+2\pi)=\phi(\theta)+2\pi$, $U$ is single-valued and $2\pi$-periodic behind the wavefront. Ahead of the first characteristic, where $\phi<0$, the fluid remains undisturbed and $U=0$. The implicit relation is [Kepler equation](../../../../../../../kepler-s-equation.md); unless $\epsilon=0$, its inverse is not a pure sinusoid.

[Series reversion](../../../../../../../series-reversion.md) gives

$$
\theta=\phi+\epsilon\sin\phi+\epsilon^2\sin\phi\cos\phi+O(\epsilon^3).
$$

Expanding the cosine then gives

$$
\cos\theta
=\cos\phi-\epsilon\sin^2\phi
-\frac32\epsilon^2\sin^2\phi\cos\phi+O(\epsilon^3),
$$

and hence

$$
\boxed{U(\phi)=a\omega\left(\cos\phi-\epsilon\sin^2\phi-\frac32\epsilon^2\sin^2\phi\cos\phi+O(\epsilon^3)\right)}
\qquad(\phi>0).
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [39B](../../../39b.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
