<h1 id="j/j1/solution">Solution</h1>

↑ **Parent:** [J1](../j1.md)

[Gauss law](../../../../gauss-s-law.md) states that for outward-oriented boundary $S=\partial V$,

$$
\boxed{\int_S\mathbf E\cdot\mathbf n\,dS=\frac1{\epsilon_0}\int_V\rho\,dV}.
$$

For a continuously differentiable field and [continuous](../../../../continuous-function.md) density, the [divergence theorem](../../../../divergence-theorem.md) turns the left side into $\int_V\nabla\cdot\mathbf E$. Thus the differential law implies the integral law. Conversely, if the integral law holds for every suitable volume, the integral of $\nabla\cdot\mathbf E-\rho/\epsilon_0$ vanishes on every small ball. A nonzero [continuous](../../../../continuous-function.md) value would keep one strict sign in some small ball, a contradiction. Hence $\nabla\cdot\mathbf E=\rho/\epsilon_0$. Weaker regularity gives the corresponding almost-everywhere or distributional formulation.

For the radial field, the flux on a radius-$r$ sphere is $4\pi r^2E(r)$, while its enclosed charge is $4\pi\int_0^r s^2\rho(s)\,ds$. Therefore

$$
\boxed{E(r)=\frac1{\epsilon_0r^2}\int_0^rs^2\rho(s)\,ds}.
$$

This uses the stated density as the full charge distribution, with no additional point charge at the origin. Since it vanishes beyond $a$, the total charge is

$$
\boxed{Q=4\pi\int_0^a s^2\rho(s)\,ds},
$$

and for $r>a$ the field is $\boxed{\mathbf E=Q\mathbf e_r/(4\pi\epsilon_0r^2)}$.

## ↑ Ancestors (12)

1. [J1](../j1.md)
2. [J](../../j.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
