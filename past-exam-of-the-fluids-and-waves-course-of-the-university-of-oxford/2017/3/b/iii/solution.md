<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Seek the periodic response of a [surface gravity wave forced by a traveling bottom](../../../../../surface-gravity-wave-forced-by-a-traveling-bottom.md), with the same [wavenumber](../../../../../wavenumber.md) $k$ and [angular frequency](../../../../../angular-frequency.md) $kc$ as the bottom. The linear equations have constant coefficients in $x,t$, so they preserve each such harmonic. There is no dissipative phase lag in this model; away from [resonance](../../../../../resonance.md), the surface response is in phase or in opposition with the bottom. Thus write $\eta=b\sin\theta$, $\theta=k(x-ct)$, with a signed coefficient $b$. Its physical [amplitude](../../../../../wave-amplitude.md) is $|b|$. Arbitrary additional free [surface gravity waves](../../../../../surface-gravity-wave.md) depend on initial data; the paper's expression selects the forced traveling component.

For $k>0$, $c\ne0$, use $\phi=F(y)\cos\theta$. The [Laplace equation](../../../../../laplace-equation.md) gives $F''-k^2F=0$. At $y=0$, the two [linearized free-surface boundary conditions](../../../../../linearized-free-surface-boundary-conditions.md) imply

$$
kcF(0)+gb=0,\qquad F'(0)=-kcb.
$$

These determine both constants in the vertical solution:

$$
\boxed{\phi(x,y,t)=-\frac b{kc}\left[g\cosh(ky)+kc^2\sinh(ky)\right]\cos(k(x-ct)).}
$$

Its vertical derivative at the bottom is

$$
\phi_y(x,-d,t)=\left[\frac{gb}{c}\sinh(kd)-kcb\cosh(kd)\right]\cos\theta.
$$

Matching it to $-akc\cos\theta$ and multiplying by $c$ gives

$$
b\left[kc^2\cosh(kd)-g\sinh(kd)\right]=akc^2,
$$

and therefore

$$
\boxed{b=\frac{akc^2}{kc^2\cosh(kd)-g\sinh(kd)}.}
$$

An equivalent expression for the [velocity potential](../../../../../velocity-potential.md), which makes the bottom condition immediate, is

$$
\phi=\left[D\cosh(k(y+d))-ac\sinh(k(y+d))\right]\cos\theta,\qquad
D=\frac c{\sinh(kd)}\left[a\cosh(kd)-b\right].
$$

Let $\omega_f=kc$ be the forcing [angular frequency](../../../../../angular-frequency.md), and let $\omega_0^2=gk\tanh(kd)$ be the natural [dispersion relation](../../../../../dispersion-relation-split.md) from [Airy wave theory](../../../../../airy-wave-theory.md). Then

$$
\frac ba=\frac{\omega_f^2\operatorname{sech}(kd)}{\omega_f^2-\omega_0^2}.
$$

The denominator vanishes at $c^2=(g/k)\tanh(kd)$, when the forcing travels at the free-wave [phase velocity](../../../../../phase-velocity.md). For nonzero forcing there is **no bounded periodic forced solution at [resonance](../../../../../resonance.md)**; the undamped linear response develops secular growth. Below that speed $b<0$, giving a phase reversal, while above it $b>0$. At $c=0$ the bottom is stationary: the rest solution has $\phi=0$ and $\eta=0$, consistent with the zero limit of $b$, though the formula containing $1/c$ must be interpreted through that limit.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
