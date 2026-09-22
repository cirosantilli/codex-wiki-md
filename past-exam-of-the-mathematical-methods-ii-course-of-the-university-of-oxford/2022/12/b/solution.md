<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand the initial [velocity](../../../../velocity.md) in the [Fourier sine basis](../../../../fourier-sine-basis.md), $V(x)=\sum_{n\ge1}V_n\sin(n\pi x/L)$, where $V_n=(2/L)\int_0^LV(x)\sin(n\pi x/L)\,dx$. Zero initial [displacement](../../../../displacement.md) removes the cosine-in-time coefficients. Thus

$$
\boxed{y(x,t)=\sum_{n\ge1}\frac{V_n}{\omega_n}\sin\frac{n\pi x}{L}\sin(\omega_nt).}
$$

The [trigonometric identity](../../../../trigonometric-identity.md) $2\sin a\sin b=\cos(a-b)-\cos(a+b)$ rewrites each summand as

$$
\frac{V_n}{2\omega_n}\left[\cos\left(\frac{n\pi x}{L}-\omega_nt\right)-\cos\left(\frac{n\pi x}{L}+\omega_nt\right)\right].
$$

It is therefore a superposition of [travelling waves](../../../../travelling-wave.md) of [speeds](../../../../speed.md) $+c$ and $-c$, whose interference enforces the fixed endpoints. For general square-integrable initial [velocity](../../../../velocity.md), the series is interpreted in the standard finite-energy sense.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [12](../../12.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
