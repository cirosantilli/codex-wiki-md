<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [arc length](../../../../../arc-length.md) $s$ as the [affine parameter](../../../../../affine-parameter.md), and put a dot over derivatives with respect to $s$. The [geodesic Lagrangian](../../../../../geodesic-lagrangian.md) on the [sphere](../../../../../sphere.md) is

$$
L=\frac{a^2}{2}(\dot\theta^2+\sin^2\theta\,\dot\phi^2).
$$

The [cyclic coordinate](../../../../../cyclic-coordinate.md) $\phi$ gives $\partial L/\partial\dot\phi=a^2\sin^2\theta\,\dot\phi=\text{constant}$. With the constant normalized as in the paper,

$$
\boxed{\sin^2\theta\,\dot\phi=h.}
$$

Here $h$ has units of inverse length, because $s$ is physical [arc length](../../../../../arc-length.md). Unit-speed normalization gives

$$
a^2\dot\theta^2+\frac{a^2h^2}{\sin^2\theta}=1.
$$

For $h\ne0$, division by $\dot\phi^2$ yields the [spherical-geodesic first integral](../../../../../spherical-geodesic-first-integral.md)

$$
\boxed{\left(\frac{d\theta}{d\phi}\right)^2+V_1(\theta)=0,
\qquad V_1(\theta)=\sin^2\theta-\frac{\sin^4\theta}{a^2h^2}.}
$$

The turning latitudes satisfy $\sin\theta=|ah|$. In the usual polar-coordinate range $0\le\theta\le\pi$,

$$
\boxed{\theta_{\min}=\arcsin|ah|,\qquad
\theta_{\max}=\pi-\arcsin|ah|,\qquad 0<|ah|\le1.}
$$

The maximum departure from the equator, often the geometric quantity intended by an angular amplitude, is instead

$$
\boxed{\max|\theta-\pi/2|=\arccos|ah|.}
$$

Thus **[polar angle](../../../../../polar-angle.md) and signed latitude must not be interchanged**. At $|ah|=1$ the [geodesic](../../../../../geodesic.md) is the equator. At $h=0$ it is a meridian through the poles; $\phi$ cannot serve as a global parameter and the divided equation is inapplicable. The limiting polar range is then $[0,\pi]$.

The original PDF prints an ambiguous derivative with the square on $\theta$ rather than a conventional derivative notation. If the intended equation was second order, differentiating the first integral, or eliminating $\dot\theta$ from the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md), gives the equally useful form

$$
\boxed{\frac{d^2\theta}{d\phi^2}+V_2(\theta)=0,\qquad
V_2(\theta)=\sin\theta\cos\theta-
\frac{2\sin^3\theta\cos\theta}{a^2h^2}.}
$$

It has the same normalized [geodesics](../../../../../geodesic.md) and the same turning angles. Giving both forms resolves the typographical ambiguity without pretending that a second derivative is the square of a first derivative. Geometrically these trajectories are [great circles](../../../../../great-circle.md), with inclination $\arccos|ah|$ to the equator.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the relativity course of the University of Cambridge](../../../../split.md)
6. [Relativity course of the University of Cambridge](../../../../../relativity-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
