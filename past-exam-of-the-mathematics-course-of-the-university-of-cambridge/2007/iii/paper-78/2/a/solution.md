<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

When [pressure](../../../../../../pressure.md) is uniform along the bubble, its normal-stress relation is $2\mu a_t=Pa-\gamma$. Use the PDF's amplitude convention $a=f+\sqrt2\,g\sin kz$; the square root acts on $2$ only, not on $2g$. Comparing constant and sinusoidal terms gives

$$
2\mu\dot f=Pf-\gamma,\qquad 2\mu\dot g=Pg.
$$

The mean cross-sectional area of an incompressible periodic segment is proportional to $\langle a^2\rangle=f^2+g^2$ and is conserved. Thus

$$
\boxed{\alpha_0=f(0)^2+g(0)^2=f(t)^2+g(t)^2.}
$$

Its time derivative vanishes, and substitution of the preceding two equations gives $P\alpha_0=\gamma f$. Therefore the [uniform-pressure evolution of a slender viscous bubble](../../../../../../uniform-pressure-evolution-of-a-slender-viscous-bubble.md) is

$$
\boxed{P=\frac{\gamma f}{\alpha_0},\qquad\dot f=-\frac{\gamma g^2}{2\mu\alpha_0},\qquad\dot g=\frac{\gamma fg}{2\mu\alpha_0}.}
$$

For a small disturbance to radius $a_0$, $f=a_0+O(g^2)$ and $\alpha_0=a_0^2+O(g^2)$, so its amplitude grows as $g\propto e^{st}$ with

$$
\boxed{s=\frac\gamma{2\mu a_0}.}
$$

The leading long-wave growth rate is independent of $k$ because axial curvature has been neglected; this is not a finite-wavelength dispersion relation.

While $f>\sqrt2g>0$, the minimum radius is $a_{\min}=f-\sqrt2g$. Its derivative is

$$
\boxed{\dot a_{\min}=-\frac\gamma{2\mu\alpha_0}(g^2+\sqrt2fg)<0.}
$$

Thus the minimum keeps decreasing in the nonlinear uniform-[pressure](../../../../../../pressure.md) model, with no need to solve $f,g$ explicitly. Finite internal viscosity eventually invalidates this model close enough to the neck.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
