<h1 id="39c/solution">Solution</h1>

↑ **Parent:** [39C](../39c.md)

For a [Fourier mode](../../../../../fourier-mode.md) $e^{i(kx-\omega t)}$, the wave equation gives

$$
-(1+k^2)^2\omega^2+k^4=0.
$$

Taking the positive-frequency branch,

$$
\boxed{\omega(k)=\frac{k^2}{1+k^2}}.
$$

For $k>0$, the [phase velocity and group velocity](../../../../../phase-velocity-and-group-velocity.md) are

$$
c_p(k)=\frac{k}{1+k^2},
\qquad
c_g(k)=\frac{2k}{(1+k^2)^2}.
$$

The frequency rises from zero and approaches $1$; $c_p$ reaches its maximum at $k=1$, while

$$
c_g'(k)=\frac{2(1-3k^2)}{(1+k^2)^3}
$$

shows that the front velocity is

$$
V_m=c_g(1/\sqrt3)=\frac{3\sqrt3}{8}.
$$

Thus the wave at the front has

$$
\boxed{k=1/\sqrt3}.
$$

Moreover $c_g/c_p=2/(1+k^2)$, so the packet outruns its crests for $0<k<1$, the speeds agree at $k=1$, and the crests outrun the packet for $k>1$.

The initial conditions give the exact superposition

$$
\varphi(x,t)=\int_{-\infty}^{\infty}A(k)
\left[e^{i(kx-\omega(k)t)}+e^{i(kx+\omega(k)t)}\right]dk.
$$

The condition $A^*(-k)=A(k)$ makes this solution real. For $V=x/t$ with $0<V<V_m$, the equation

$$
\boxed{V=\omega'(\alpha)=\frac{2\alpha}{(1+\alpha^2)^2}}
$$

has two positive roots $0<\alpha_1<1/\sqrt3<\alpha_2$. The second exponential has the corresponding stationary points $-\alpha_1,-\alpha_2$. Since

$$
\omega''(k)=\frac{2(1-3k^2)}{(1+k^2)^3},
$$

the [stationary phase method](../../../../../stationary-phase-method.md) and pairing of complex-conjugate contributions give

$$
\boxed{
\varphi(Vt,t)\sim2\operatorname{Re}\sum_{j=1}^2
\left(\frac{2\pi}{t|\omega''(\alpha_j)|}\right)^{1/2}
A(\alpha_j)
\exp\left\{it[\alpha_jV-\omega(\alpha_j)]
-\frac{i\pi}{4}\operatorname{sgn}\omega''(\alpha_j)\right\}
}.
$$

For $-V_m<V<0$, the same picture is reflected and the stationary points have negative wavenumber. For $|V|>V_m$ there are no real stationary points, so a smooth localized spectrum gives a much smaller nonstationary tail outside the wave front.

## ↑ Ancestors (10)

1. [39C](../39c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
