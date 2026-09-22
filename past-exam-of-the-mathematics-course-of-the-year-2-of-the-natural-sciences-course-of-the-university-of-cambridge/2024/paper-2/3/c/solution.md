<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Green's second identity](../../../../../green-second-identity.md), with the outward [normal derivative](../../../../../normal-derivative.md), is

$$
\int_S(u\Delta v-v\Delta u)\,dS
=\oint_C\left(u\frac{\partial v}{\partial n}-v\frac{\partial u}{\partial n}\right)dC.
$$

Set $u=\Phi$ and $v=G(\cdot;\mathbf r')$, interpreting the logarithmic singularity by a small excised disc or [distribution theory](../../../../../distribution-theory-split.md). The volume integral is $\Phi(\mathbf r')$ because $\Delta\Phi=0$ and $\Delta G=\delta$. On the boundary $G=0$ and $\Phi=f$, leaving

$$
\boxed{\Phi(\mathbf r')=\oint_C f(\mathbf r)\frac{\partial G(\mathbf r;\mathbf r')}{\partial n}\,dC.}
$$

For the exterior problem below, apply the identity first in a large truncated region. For bounded [harmonic functions](../../../../../harmonic-function.md) the extra circle at infinity contributes zero: $G$ tends to a constant, its radial derivative is $O(r^{-2})$, and a bounded exterior [harmonic function](../../../../../harmonic-function.md) also has radial derivative $O(r^{-2})$. This is the condition under which the same boundary representation applies there.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
