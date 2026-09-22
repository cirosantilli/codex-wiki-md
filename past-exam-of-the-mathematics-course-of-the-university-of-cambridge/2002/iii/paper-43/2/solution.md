<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose the [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) convention $\mathbf B_p=\nabla\times(A\hat{\mathbf y})=(-A_z,0,A_x)$. The term $\alpha B$ regenerates this poloidal flux function from the [toroidal magnetic field](../../../../../toroidal-magnetic-field.md) through the [alpha effect](../../../../../alpha-effect.md). It represents a component of the [mean-field electromotive force](../../../../../mean-field-electromotive-force.md) produced by correlated [velocity](../../../../../velocity.md) and magnetic fluctuations. The shear $G=\pi V/d$ stretches the poloidal vertical component $B_{p,z}=A_x$ into toroidal field, giving $GA_x$: this is the [Omega effect](../../../../../omega-effect.md). Both $\eta\nabla^2$ terms diffuse and damp the field. In a turbulent mean-field model, $\eta$ can denote an effective diffusivity including turbulent transport. The [alpha-Omega dynamo](../../../../../alpha-omega-dynamo.md) approximation retains the shear-dominated toroidal source, and the [kinematic dynamo](../../../../../kinematic-magnetic-dynamo.md) assumption prescribes the [velocity](../../../../../velocity.md) and coefficients without their [Lorentz force](../../../../../lorentz-force.md) feedback.

For a horizontal [wavenumber](../../../../../wavenumber.md) $k$ and vertical [wavenumber](../../../../../wavenumber.md) $\pi/d$, set $K^2=k^2+\pi^2/d^2$ and seek amplitudes proportional to $e^{st}$. The two modal equations are

$$
(s+\eta K^2)\widehat A=\alpha\widehat B,
\qquad(s+\eta K^2)\widehat B=ikG\widehat A.
$$

A nonzero mode requires the [dispersion relation](../../../../../dispersion-relation.md)

$$
(s+\eta K^2)^2=i\alpha Gk.
$$

For real nonzero $\alpha Gk$, the root with positive real square-root part is

$$
s_+=-\eta K^2+\sqrt{\frac{|\alpha Gk|}{2}}
\left(1+i\operatorname{sgn}(\alpha Gk)\right).
$$

The other root has strictly negative real part. For $k=0$ there is no oscillatory feedback and both roots have real part $-\eta\pi^2/d^2$; the possible triangular-system prefactor cannot yield exponential growth.

Let $h=|k|d/\pi>0$ and $D=\alpha Vd^2/(\pi^2\eta^2)$. The growing-branch exponent satisfies

$$
\frac{\Re s_+}{\eta\pi^2/d^2}
=-(1+h^2)+\sqrt{\frac{|D|h}{2}}.
$$

Consequently the [plane-layer alpha-Omega dynamo threshold](../../../../../plane-layer-alpha-omega-dynamo-threshold.md) at fixed $h$ is

$$
|D|>D_c(h):=\frac{2(1+h^2)^2}{h}.
$$

To find its least value, differentiate $D_c(h)=2(h^{-1}+2h+h^3)$:

$$
D_c'(h)=2(-h^{-2}+2+3h^2)=0
\quad\Longleftrightarrow\quad3h^4+2h^2-1=0.
$$

The unique positive solution is $h^2=1/3$. The threshold diverges at both ends $h\downarrow0$ and $h\to\infty$, so this is its global minimum. Hence

$$
\boxed{|D|_c=\frac{32}{3\sqrt3},\qquad
|k_c|=\frac{\pi}{\sqrt3\,d}.}
$$

With the usual positive-$D$ convention, the onset value is $D_c=32/(3\sqrt3)$ and exponentially growing waves exist for $D>D_c$. Exactly at the threshold the real part is zero, so it is a neutral dynamo wave: the quoted minimum is the onset threshold, or infimum for strict growth, not a growing solution at equality. If signed $D$ is allowed, the growth condition concerns $|D|$; there is no smallest signed negative value among all growing cases.

The real field is obtained by taking the real part of a [Fourier mode](../../../../../fourier-mode.md). Its phase is $kx+(\Im s_+)t+\pi z/d$, so the horizontal phase speed is $-(\Im s_+)/k$. Reversing the sign of $\alpha V$ reverses propagation, while leaving the growth threshold unchanged. Reversing $k$ gives the conjugate real-field representation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
