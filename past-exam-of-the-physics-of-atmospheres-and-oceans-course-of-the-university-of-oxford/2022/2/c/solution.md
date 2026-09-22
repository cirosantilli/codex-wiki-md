<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\tau_0=\tau_\infty$, $n=2a$, and $t=\tau_0(p/p_s)^2$. The integrated [Planck function](../../../../planck-function.md) is $B(T)=\sigma T^4/\pi$ by the [Stefan–Boltzmann law](../../../../stefan-boltzmann-law.md), and

$$
B(t)=\frac{\sigma T_s^4}{\pi}\left(\frac t{\tau_0}\right)^n.
$$

The formal [radiative transfer equation](../../../../radiative-transfer-equation.md) solution for upward [radiance](../../../../radiance.md) at the top is

$$
I(0,\mu)=\frac{\sigma T_s^4}{\pi}e^{-\tau_0/\mu}
+\int_0^{\tau_0}B(t)e^{-t/\mu}\frac{dt}{\mu},\qquad0<\mu\leq1.
$$

The first term is transmitted surface emission; the second is emission from the [atmosphere](../../../../atmosphere.md). Integrating [radiance](../../../../radiance.md) over the upward hemisphere gives the outgoing [radiant flux](../../../../radiant-flux.md) per unit area,

$$
\boxed{F=2\sigma T_s^4\left[E_3(\tau_0)+\tau_0^{-n}
\int_0^{\tau_0}t^nE_2(t)\,dt\right],\qquad
E_j(t)=\int_0^1\mu^{j-2}e^{-t/\mu}\,d\mu.}
$$

Here $E_j$ is an [exponential integral](../../../../exponential-integral.md). For fixed $a$ and $\tau_0\to\infty$, surface transmission is negligible and the upper limit can be extended to infinity. Positivity permits interchanging the [integrals](../../../../integral-split.md); putting $t=\mu x$ gives

$$
\int_0^\infty t^nE_2(t)\,dt
=\int_0^1\mu^{n+1}\,d\mu\int_0^\infty x^ne^{-x}\,dx
=\frac{\Gamma(n+1)}{n+2}.
$$

Consequently the exact hemispheric optically thick result is

$$
\boxed{F\sim\sigma T_s^4\tau_0^{-2a}\,
\frac{\Gamma(2a+1)}{a+1}.}
$$

This is a dimensional scale times a dimensionless definite [integral](../../../../integral-split.md) depending only on $a$. In the commonly used vertical-ray approximation, define $F_{\rm v}=\pi I(0,1)$. Then

$$
F_{\rm v}=\sigma T_s^4\left[e^{-\tau_0}+\tau_0^{-2a}\int_0^{\tau_0}t^{2a}e^{-t}\,dt\right]
\sim\sigma T_s^4\tau_0^{-2a}\Gamma(2a+1).
$$

A vertical-ray approximation therefore has the same scaling but omits the angular factor $1/(a+1)$. Stating which quantity is used prevents a purely angular normalization discrepancy.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
