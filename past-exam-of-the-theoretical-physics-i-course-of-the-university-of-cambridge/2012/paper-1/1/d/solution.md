<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The time-independent [Lagrangian](../../../../../lagrangian.md) conserves $E=T+V$. Substitute $\dot x=-m_2l\dot\phi\cos\phi/M$ into the [kinetic energy](../../../../../kinetic-energy.md) to obtain

$$
\boxed{E=\frac{m_2l^2}{2M}(m_1+m_2\sin^2\phi)\dot\phi^2-m_2gl\cos\phi.}
$$

This is the angle-dependent effective inertia of a [pendulum with a freely sliding support](../../../../../pendulum-with-a-freely-sliding-support.md). Solving for the speed gives

$$
|\dot\phi|=\sqrt{\frac{2M(E+m_2gl\cos\phi)}{m_2l^2(m_1+m_2\sin^2\phi)}}.
$$

On a monotone increasing segment, the travel time is therefore

$$
\boxed{t=l\sqrt{\frac{m_2}{2M}}\int_{\phi_1}^{\phi_2}
\sqrt{\frac{m_1+m_2\sin^2\phi}{E+m_2gl\cos\phi}}\,d\phi.}
$$

The printed oriented [integral](../../../../../integral-split.md) assumes that increasing-angle branch. For decreasing motion use $|d\phi|$ or interchange the limits; if a [turning point](../../../../../turning-point.md) lies between the two events, split the trajectory into monotone segments and add their positive times. The numerator remains positive for positive masses. At an ordinary [turning point](../../../../../turning-point.md) the inverse-square-root singularity is integrable; reaching the unstable upright [separatrix](../../../../../separatrix.md) takes infinite time.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
