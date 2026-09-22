<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the relative coordinate and [reduced mass](../../../../../reduced-mass.md)

$$
\mu=\frac{m_pm_n}{m_p+m_n},\qquad \mu c^2=469.459\,\mathrm{MeV}.
$$

Take $V=-V_0$ inside, $V=0$ outside, and $E=-B$. For $V_0>B>0$, define inverse lengths

$$
k=\frac{\sqrt{2\mu c^2(V_0-B)}}{\hbar c},\qquad
\kappa=\frac{\sqrt{2\mu c^2B}}{\hbar c}.
$$

The radial equation becomes $u''+k^2u=0$ inside and $u''-\kappa^2u=0$ outside. Finiteness of the full [wavefunction](../../../../../wave-function-split.md) at the origin imposes $u(0)=0$; normalizability excludes the growing exterior exponential. Hence

$$
u(r)=A\begin{cases}
\sin(kr),&0\leq r\leq b,\\
\sin(kb)e^{-\kappa(r-b)},&r\geq b.
\end{cases}
$$

Continuity of $u$ was built in. Continuity of its derivative at the finite step gives

$$
\boxed{k\cot(kb)=-\kappa,\qquad k^2+\kappa^2=\frac{2\mu c^2V_0}{(\hbar c)^2}.}
$$

For the nodeless [ground state](../../../../../ground-state.md), $\pi/2<kb<\pi$ selects the first branch. Higher roots would correspond to different wells with more [bound states](../../../../../bound-state.md). Normalization is

$$
A^{-2}=\frac b2-\frac{\sin(2kb)}{4k}+\frac{\sin^2(kb)}{2\kappa}.
$$

For the requested weak-binding estimate, $B/V_0\to0$ makes $\kappa/k\to0$. On the first branch $kb\to\pi/2$, and $k^2\simeq2\mu c^2V_0/(\hbar c)^2$. The leading threshold estimate is

$$
\boxed{V_0\simeq\frac{\pi^2(\hbar c)^2}{8\mu c^2b^2}
=\frac{\pi^2(197.3)^2}{8(469.459)(2.1)^2}\,\mathrm{MeV}
=23.2\,\mathrm{MeV}.}
$$

This is the zero-binding threshold of a [spherical square well](../../../../../spherical-square-well.md), so nonzero positive binding needs a depth above it. Corrections start at order $\sqrt B$, not just at order $B$: setting $kb=\pi/2+\epsilon$ gives $\epsilon\simeq\kappa b/(\pi/2)$ and

$$
V_0\simeq V_{\rm threshold}+\frac{(\hbar c)^2\kappa}{\mu c^2b}+O(B)
\simeq32.3\,\mathrm{MeV}+O(B).
$$

The actual numbers permit an accuracy check: $\kappa=0.231608\,\mathrm{fm}^{-1}$ and $\kappa b=0.486377$ are not extremely small. Retaining the exterior decay, solve

$$
x\cot x=-0.486377,\qquad \pi/2<x<\pi.
$$

This gives $x=kb=1.830503$, and the full square-well result is

$$
V_0=B+\frac{(\hbar c)^2x^2}{2\mu c^2b^2}
=\boxed{33.73\,\mathrm{MeV}\quad\text{without weak-binding truncation}.}
$$

Neglecting $B$ only in the interior kinetic relation while retaining the measured exterior decay instead estimates $V_0\simeq31.50\,\mathrm{MeV}$. These approximations should be identified: 23.2 MeV is the leading $B\to0$ threshold, whereas matching the supplied nonzero binding requires a boundary phase shift and a deeper well.

<a id="4/d/image-a-weakly-bound-radial-state-extends-beyond-the-finite-nuclear-well"></a>
![](../../../../../past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2016/paper-1-deuteron-well.png)

**[Figure 4](#4/d/image-a-weakly-bound-radial-state-extends-beyond-the-finite-nuclear-well). A weakly bound radial state extends beyond the finite nuclear well**. Original calculation from the stated [masses](../../../../../mass.md), radius and binding. The reduced radial function is normalized with $\int_0^\infty|u|^2dr=1$ and matches its derivative at the well edge. The central-well model omits the tensor-induced D component.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the particle and nuclear physics course of the University of Cambridge](../../../../split.md)
6. [Particle and Nuclear Physics course of the University of Cambridge](../../../../../particle-and-nuclear-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
