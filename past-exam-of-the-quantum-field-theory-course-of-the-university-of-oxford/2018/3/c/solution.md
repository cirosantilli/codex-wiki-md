<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In four dimensions set $b=3/(16\pi^2)$ and retain the one-loop [beta function](../../../../beta-function.md) $dg/d\log\mu=bg^2$. On an interval where $g\ne0$, differentiate its inverse:

$$
\frac{d(1/g)}{d\log\mu}=-b.
$$

Integrating between $\mu_s$ and $\mu$ yields

$$
\frac1{g(\mu)}=\frac1{g_s}-b\log\frac\mu{\mu_s},\qquad
\boxed{g(\mu)=\frac{g_s}{1-\dfrac{3g_s}{16\pi^2}\log(\mu/\mu_s)}.}
$$

The $g_s=0$ solution is identically zero and is also the continuous limit of this expression. Expanding the denominator gives $g(\mu)=g_s+bg_s^2\log(\mu/\mu_s)+\cdots$, directly checking the perturbative sign.

For positive $g_s$, the [running coupling](../../../../running-coupling.md) decreases towards the infrared and increases towards the ultraviolet. The one-loop expression has a [Landau pole](../../../../landau-pole.md) at

$$
\mu_L=\mu_s\exp\left(\frac{16\pi^2}{3g_s}\right).
$$

This is the scale where the truncated solution diverges, not a controlled perturbative prediction of a physical singularity at arbitrarily strong coupling. The formula is quantitatively reliable while the running coupling remains small enough that omitted higher-loop terms are negligible. It resums the leading logarithms of that approximate [renormalization group](../../../../renormalization-group.md) equation; it is not the exact all-orders solution of the theory.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
