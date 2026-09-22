<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

Substitution of $e^{i(kx-\omega t)}$ in the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) gives $\boxed{\omega^2=1+k^2}$. On the positive-frequency branch, the [phase velocity](../../../../../phase-velocity.md) is $\boxed{c_p=\sqrt{1+k^2}/k}$ for $k\ne0$, and the [group velocity](../../../../../group-velocity.md) is $\boxed{c_g=k/\sqrt{1+k^2}}$. The group speed is less than one, although the phase speed exceeds one in magnitude.

With [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(k)=\int f(x)e^{-ikx}\,dx$, the initial velocity has transform $2/(1+k^2)$. Each Fourier mode solves a harmonic-oscillator equation, giving

$$
\boxed{\phi(x,t)=\frac1\pi\int_{-\infty}^{\infty}\frac{e^{ikx}\sin(t\sqrt{1+k^2})}{(1+k^2)^{3/2}}\,dk.}
$$

For $x=Vt$, symmetry makes this the imaginary part of $\pi^{-1}\int(1+k^2)^{-3/2}e^{it(\sqrt{1+k^2}-Vk)}\,dk$. When $0<V<1$, the phase has a unique stationary point $k_*=V/\sqrt{1-V^2}$, with phase value $\sqrt{1-V^2}$ and positive second derivative $(1-V^2)^{3/2}$. The [stationary phase](../../../../../stationary-phase-method.md) method gives

$$
\boxed{\phi(Vt,t)=\sqrt{\frac2{\pi t}}(1-V^2)^{3/4}\sin\left(t\sqrt{1-V^2}+\frac\pi4\right)+O(t^{-3/2}).}
$$

For $V>1$ there is no real stationary point. More precisely, [finite propagation speed](../../../../../finite-propagation-speed.md) makes the solution at $x>t$ depend only on the initial data on $[x-t,x+t]\subset(0,\infty)$. On that half-line the initial velocity is $e^{-x}$, and $te^{-x}$ exactly solves the equation with zero initial displacement. Uniqueness on the domain of dependence therefore gives

$$
\boxed{\phi(Vt,t)=te^{-Vt}\quad(V>1).}
$$

This [exponential initial-velocity tail for the Klein-Gordon equation](../../../../../exponential-initial-velocity-tail-for-the-klein-gordon-equation.md) is exponentially small, rather than identically zero: the initial data already have a nonzero tail outside the origin.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
