<h1 id="39a/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Each Fourier mode has zero initial velocity, so

$$
\phi(x,t)=\int_{-\infty}^{\infty}a(k)e^{ikx}\cos(\omega(k)t)\,dk.
$$

Along $x=Vt$ this is

$$
\phi(Vt,t)=\frac12\int_{-\infty}^{\infty}a(k)
\left[e^{it(kV+\omega(k))}+e^{it(kV-\omega(k))}\right]dk.
$$

Put

$$
s=\sqrt{c^2-V^2},
\qquad
k_0=\frac{AV}{s}.
$$

The two phases have stationary points at $-k_0$ and $k_0$, respectively. At those points,

$$
k_0V-\omega(k_0)=-As,
\qquad
\omega''(k_0)=\frac{s^3}{Ac^2}.
$$

Because the initial field is real, $a(-k)=a(k)^*$. Applying the [stationary phase method](../../../../../../../stationary-phase-method.md) to the two conjugate contributions gives the [stationary-phase asymptotic of a Klein-Gordon wave along a subluminal ray](../../../../../../../stationary-phase-asymptotic-of-a-klein-gordon-wave-along-a-subluminal-ray.md):

$$
\boxed{
\phi(Vt,t)\sim
\left(\frac{2\pi Ac^2}{t s^3}\right)^{1/2}
\operatorname{Re}\left\{
a(k_0)e^{-i(As t+\pi/4)}
\right\}.}
$$

Equivalently, if $a(k_0)=|a(k_0)|e^{i\delta}$,

$$
\phi(Vt,t)\sim
|a(k_0)|\left(\frac{2\pi Ac^2}{t s^3}\right)^{1/2}
\cos\left(As t+\frac\pi4-\delta\right).
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [39A](../../../39a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
