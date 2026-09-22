<h1 id="d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

A [travelling wave](../../../../travelling-wave.md), for example $A\cos(kx-\omega t)$, has moving constant-phase surfaces. A [standing wave](../../../../standing-wave.md), for example $2A\sin(kx)\cos(\omega t)$, has stationary [nodes](../../../../node-dynamical-systems.md) and can be formed from two equal counterpropagating waves.

For the [half-line finite well](../../../../half-line-finite-well.md) with $E>V_0$, define $k=\sqrt{2mE}/\hbar$ and $q=\sqrt{2m(E-V_0)}/\hbar$. The hard wall requires $\psi=0$ for $x<0$ and $\psi(0)=0$, so the general allowed forms are

$$
\boxed{\psi(x)=\begin{cases}
0,&x<0,\\
A\sin(kx),&0<x<a,\\
Be^{iq(x-a)}+Ce^{-iq(x-a)},&x>a.
\end{cases}}
$$

At the finite step both $\psi$ and $\psi'$ are continuous:

$$
A\sin(ka)=B+C,\qquad Ak\cos(ka)=iq(B-C).
$$

There is no requirement to match the derivative to zero across the infinite wall.

For a [bound state](../../../../bound-state.md) $0<E<V_0$, put $\kappa=\sqrt{2m(V_0-E)}/\hbar>0$. Normalizability excludes the growing exponential, leaving $A\sin(kx)$ inside and $De^{-\kappa(x-a)}$ outside. Matching their logarithmic derivatives gives

$$
\boxed{k\cot(ka)=-\kappa,\qquad \tan(ka)=-k/\kappa.}
$$

The exterior expression is equivalent to $Ce^{-\kappa x}$ by rescaling its constant. Negative cotangent first occurs for $\pi/2<ka<\pi$; all higher allowed intervals also have $ka>\pi/2$. Thus $\lambda_1=2\pi/k<4a$. Since $k<\sqrt{2mV_0}/\hbar$, a normalizable [bound state](../../../../bound-state.md) requires

$$
\boxed{V_0>\frac{\pi^2\hbar^2}{8ma^2}.}
$$

This is also sufficient: on the lowest negative-cotangent branch, the two matching sides cross whenever $a\sqrt{2mV_0}/\hbar>\pi/2$. **The printed non-strict inequality includes the threshold limit.** At equality $E=V_0$ and the exterior is not square-integrable, so it is not itself a [bound state](../../../../bound-state.md).

For the helium [mass](../../../../mass.md) and [energy](../../../../energy-split.md) scale given, the limiting width is

$$
\boxed{a_{\rm th}=\frac{\pi\hbar}{\sqrt{8m_{\rm He}V_0}}=1.14\times10^{-10}\,\mathrm m=0.114\,\mathrm{nm}.}
$$

Actual binding requires a width just larger than this threshold in the stated ideal potential.

## ↑ Ancestors (12)

1. [D12](../d12.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
