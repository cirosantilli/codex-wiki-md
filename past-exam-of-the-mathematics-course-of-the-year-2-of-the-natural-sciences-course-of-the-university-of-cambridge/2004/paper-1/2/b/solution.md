<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [Fourier's law](../../../../../fourier-s-law.md), insulation means zero outward heat flux. The [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) are $\theta_x(0,t)=\theta_x(L,t)=0$. The constant mode equals the initial [integral average](../../../../../integral-average.md) $L/4$. For $n\geq1$, the cosine coefficients are

$$
a_n=\frac{2L}{n^2\pi^2}\left[2\cos\frac{n\pi}{2}-1-(-1)^n\right].
$$

Odd modes and modes divisible by four vanish; write the remaining indices as $n=2(2j+1)$. The [heat flow from a triangular initial temperature with insulated endpoints](../../../../../heat-flow-from-a-triangular-initial-temperature-with-insulated-endpoints.md) gives

$$
\boxed{\theta_N(x,t)=\frac L4-\frac{2L}{\pi^2}\sum_{j=0}^\infty\frac{\cos(2(2j+1)\pi x/L)}{(2j+1)^2}\,e^{-\nu[2(2j+1)\pi/L]^2t}.}
$$

The nonconstant modes decay, so $\boxed{\theta_N\to L/4}$ uniformly as $t\to\infty$. Integrating the [heat equation](../../../../../heat-equation.md) gives $d(\int_0^L\theta\,dx)/dt=\nu[\theta_x]_0^L=0$, explaining the conserved mean. The cooled case tends instead to zero because heat leaves through its ends.

The initial triangle has nonzero endpoint slopes, so it is not compatible with the insulated condition at the corner $t=0$. The series nevertheless recovers the continuous initial temperature and satisfies the insulated condition for every $t>0$; one should not assert continuity of its spatial derivative at that initial corner.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
