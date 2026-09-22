<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There are two different physical interpretations. The supplied logarithmic integral signals [free fall in a fixed singular isothermal sphere](../../../../free-fall-in-a-fixed-singular-isothermal-sphere.md), with a test particle moving through a frozen background. Write $C=\rho_0r_0^2$. By the [shell theorem](../../../../spherical-shell-theorem.md), the enclosed [mass](../../../../mass.md) is $M(r)=4\pi Cr$ and the radial [equation of motion](../../../../equation-of-motion.md) is

$$
\ddot r=-\frac{4\pi GC}{r},\qquad
\frac{\dot r^2}{2}=4\pi GC\ln\frac{r_0}{r},\qquad \dot r<0.
$$

The second equality follows by multiplying by $\dot r$ and using the initial rest condition. The [free fall](../../../../free-fall.md) trajectory is given implicitly by

$$
t(r)=\frac{r_0}{\sqrt{8\pi GC}}\int_{r/r_0}^1\frac{dx}{\sqrt{\ln(1/x)}}
=\frac{1}{\sqrt{8G\rho_0}}\operatorname{erf}\!\sqrt{\ln(r_0/r)}.
$$

Thus the intended fixed-profile answer is

$$
\boxed{t_{\rm ff,fixed}=\frac{1}{\sqrt{8G\rho_0}}.}
$$

**A collapsing material shell gives a different answer.** If the entire cloud undergoes pressureless [gravitational collapse](../../../../gravitational-collapse.md) from rest, the edge follows the fixed enclosed [mass](../../../../mass.md) $M_0=4\pi\rho_0r_0^3$, not the instantaneous fixed-profile value $4\pi Cr$. With no [shell crossing](../../../../shell-crossing.md), $\ddot r=-GM_0/r^2$, so

$$
t_{\rm ff,shell}=\int_0^{r_0}\frac{dr}{\sqrt{2GM_0(1/r-1/r_0)}}
=\frac{\pi}{2}\sqrt{\frac{r_0^3}{2GM_0}}
=\boxed{\sqrt{\frac{\pi}{32G\rho_0}}}.
$$

This is a concrete counterexample to treating the fixed-profile result as the exact collapse time of the whole nebula. The initial mean [density](../../../../density.md) inside $r_0$ is $3\rho_0$, consistent with the usual [free-fall time of a uniform sphere](../../../../free-fall-time-of-a-uniform-sphere.md) expressed using that mean [density](../../../../density.md). The logarithmic integral is valid for the explicitly frozen background approximation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
