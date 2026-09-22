<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

After a [Wick rotation](../../../../wick-rotation.md), the term in question has radial behavior

$$
I_m=m^2\int\frac{d^4k}{(2\pi)^4}\frac1{(k^2+i0)(k^2-m^2+i0)^2}=-i\int\frac{d^4k_E}{(2\pi)^4}\frac{m^2}{k_E^2(k_E^2+m^2)^2}.
$$

The radial integrand is proportional to $k_E$ at the origin and to $k_E^{-3}$ at infinity. Thus it has neither an [infrared divergence](../../../../infrared-divergence.md) nor an [ultraviolet divergence](../../../../ultraviolet-divergence.md). In fact the area of the unit three-sphere gives

$$
I_m=-\frac{i m^2}{8\pi^2}\int_0^\infty\frac{r\,dr}{(r^2+m^2)^2}=\boxed{-\frac{i}{16\pi^2}}.
$$

This also follows from the [Feynman parameter](../../../../feynman-parameter.md) identity

$$
\frac1{AB^2}=2\int_0^1dx\,\frac{1-x}{[xA+(1-x)B]^3}
$$

with $A=k^2+i0$, $B=k^2-m^2+i0$. Although the parameterized denominator becomes massless at $x=1$, its numerator $1-x$ cancels the apparent endpoint singularity. Since $\beta\to-2$, multiplication by $\beta$ preserves finiteness. No artificial [photon](../../../../photon.md) [mass](../../../../mass.md) is needed.

## ↑ Ancestors (12)

1. [Vi](../vi.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
