<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

With the [streamfunction](../../../../../stream-function.md) convention $(u,v)=(\psi_y,-\psi_x)$, disturbance [vorticity](../../../../../vorticity.md) is $\omega=-\Delta\psi$. The basic [Couette flow](../../../../../couette-flow.md) has constant [vorticity](../../../../../vorticity.md) $-1$. Linearizing the two-dimensional [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) in [vorticity](../../../../../vorticity.md) form gives

$$
(\partial_t+y\partial_x)\omega+\mathbf u'\cdot\nabla(-1)=0.
$$

The second term vanishes, so

$$
\boxed{(\partial_t+y\partial_x)\Delta\psi=0.}
$$

This derivation uses incompressibility and an inviscid homogeneous fluid, without introducing a viscous decay term.

For the initial streamwise [Fourier mode](../../../../../fourier-mode.md), write $\psi=e^{i\alpha x}a(y,t)$. Its transported Laplacian has amplitude

$$
(\partial_y^2-\alpha^2)a=F(y)e^{-i\alpha yt},\qquad F(y)=\phi''(y)-\alpha^2\phi(y).
$$

The decaying [Green function](../../../../../green-s-function.md) on the line is

$$
\boxed{G(y,s)=-\frac{e^{-\alpha|y-s|}}{2\alpha},\qquad F(s)=\phi''(s)-\alpha^2\phi(s).}
$$

This is the negative of the [one-dimensional modified Helmholtz Green function](../../../../../one-dimensional-modified-helmholtz-green-function.md) for $-\partial_y^2+\alpha^2$: it is continuous and its first derivative with respect to $y$ has jump one at $y=s$. Consequently $(\partial_y^2-\alpha^2)G=\delta(y-s)$, and inversion yields

$$
\boxed{\psi(x,y,t)=\int_{\mathbb R}F(s)G(y,s)e^{i\alpha(x-st)}ds.}
$$

Under the usual decay of the initial profile and its derivatives, the initial integral returns $\phi$. There is no nonzero homogeneous solution of $a''-\alpha^2a=0$ decaying at both infinities.

For the large-time calculation, put $q=\alpha t$ and $H(s)=G(y,s)F(s)$, keeping the observation point $y$ fixed. Assume sufficient localization to justify the following [integrations by parts](../../../../../integration-by-parts.md); for example, $F$ may be a [Schwartz function](../../../../../schwartz-function.md). The function $H$ is continuous, but its derivative in $s$ has jump

$$
[H_s]_{s=y}=F(y),
$$

since $G_s(y,y+)-G_s(y,y-)=1$. The [Fourier decay from a Green-function derivative jump](../../../../../fourier-decay-from-a-green-function-derivative-jump.md) gives

$$
\int H(s)e^{-iqs}ds=-\frac1{q^2}\left[F(y)e^{-iqy}+\int H''_{\mathrm{reg}}(s)e^{-iqs}ds\right].
$$

Here the regular second derivative is computed separately on either side of $s=y$. If it is integrable, its [Fourier transform](../../../../../fourier-transform.md) tends to zero by the [Riemann-Lebesgue lemma](../../../../../riemann-lebesgue-lemma.md). Hence

$$
\boxed{\psi(x,y,t)=-\frac{F(y)}{\alpha^2t^2}e^{i\alpha(x-yt)}+o(t^{-2}).}
$$

The cusp in the [Green function](../../../../../green-s-function.md), rather than a stationary point of the linear phase, supplies this leading contribution.

To obtain the streamwise [velocity](../../../../../velocity.md), differentiate the integral itself. This avoids an unjustified differentiation of a pointwise remainder. The kernel $G_y$ has a jump of $-1$ as a function of $s$ at $s=y$, so one [integration by parts](../../../../../integration-by-parts.md) gives

$$
u(x,y,t)=e^{i\alpha x}\int G_y(y,s)F(s)e^{-iqs}ds=\frac{iF(y)}{\alpha t}e^{i\alpha(x-yt)}+o(t^{-1}).
$$

The transverse [velocity](../../../../../velocity.md) follows exactly from $v=-i\alpha\psi$, while the Laplacian equation gives [vorticity](../../../../../vorticity.md) without an asymptotic approximation:

$$
\boxed{\begin{aligned}
u(x,y,t)&=\frac{iF(y)}{\alpha t}e^{i\alpha(x-yt)}+o(t^{-1}),\\
v(x,y,t)&=\frac{iF(y)}{\alpha t^2}e^{i\alpha(x-yt)}+o(t^{-2}),\\
\omega(x,y,t)&=-F(y)e^{i\alpha(x-yt)}.
\end{aligned}}
$$

Thus the generic orders are $u=O(t^{-1})$, $v=O(t^{-2})$, and $\omega=O(1)$, at each fixed $y$. If $F(y)=0$, the leading coefficients vanish and faster decay can occur. For real physical disturbances, take the real part of these complex [Fourier modes](../../../../../fourier-mode.md). The [vorticity](../../../../../vorticity.md) generally keeps oscillating rather than approaching a pointwise limit, even while the [velocity](../../../../../velocity.md) decays. This is [linear inviscid damping in unbounded Couette flow](../../../../../linear-inviscid-damping-in-unbounded-couette-flow.md) caused by phase mixing.

For arbitrary initial [vorticity](../../../../../vorticity.md), the [characteristics](../../../../../characteristic-of-a-field.md) satisfy $\dot x=y$, $\dot y=0$, and $\dot\omega=0$. Therefore the exact solution is

$$
\boxed{\omega(x,y,t)=\omega_0(x-yt,y).}
$$

Putting $\omega_0=-F(y)e^{i\alpha x}$ recovers the preceding nondecaying mode. In general the shear is area preserving, so its transport preserves every finite [Lp norm](../../../../../lp-norm.md) of [vorticity](../../../../../vorticity.md). Local pointwise behavior for arbitrary $\omega_0$ depends on its spatial profile: an initially localized profile can move away from a fixed point. There is no universal pointwise nonzero limit or $t^{-2}$ decay of [vorticity](../../../../../vorticity.md) for arbitrary initial data.

**The stated smoothness and decay of $\phi$ alone do not guarantee the claimed algebraic rates.** The intended [integration by parts](../../../../../integration-by-parts.md) calculation requires control of derivatives and tails; convergence of the displayed integral alone is insufficient. Here is a counterexample to the literal unrestricted rate, with $\alpha=1$. Choose a nonnegative smooth function $r$ supported in $(-1/4,1/4)$ with $\int r=1$, and a sufficiently rapidly increasing sequence $t_n$. Set

$$
F(s)=\sum_{n\ge1}\frac{e^s}{t_n}r(s-n)e^{it_ns},\qquad \phi=G*F,\qquad G(s)=-\frac12e^{-|s|}.
$$

Choose $\sum e^n/t_n<\infty$. Then $F$ is smooth and integrable, $\phi$ is smooth and tends to zero at both infinities, and every evolution integral converges absolutely. At the observation point $(x,y)=(0,0)$, all supports have $s>0$, so

$$
\psi(0,0,t)=-\frac12\sum_{n\ge1}\frac1{t_n}e^{-i(t-t_n)n}\widehat r(t-t_n),\qquad \widehat r(\xi)=\int r(s)e^{-i\xi s}ds.
$$

At $t=t_n$, the $n$th summand is $-1/(2t_n)$. The [Fourier transform](../../../../../fourier-transform.md) of $r$ decays faster than any inverse power. Inductively choose $t_n$ so large that all earlier summands at $t_n$ together have modulus less than $1/(8t_n)$, and choose subsequent times so that $\sum_{m>n}1/t_m<1/(4t_n)$. The later summands then also have modulus less than $1/(8t_n)$. Thus $|\psi(0,0,t_n)|\ge1/(4t_n)$, contradicting $O(t^{-2})$. This construction meets the printed assumptions; what it lacks is uniform derivative localization. The preceding boxed decay formulas are the correct intended result under the explicitly stated sufficient localization hypothesis.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
