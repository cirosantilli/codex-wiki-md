<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Integrate the radial equilibrium equation across the thickness, retaining the [integral](../../../../integral-split.md) rather than evaluating its [antiderivative](../../../../antiderivative.md). The [traction](../../../../traction.md) conditions give $t_r(b)-t_r(a)=P$. Hence $a$ must satisfy

$$
\boxed{P=\mu\int_a^{\sqrt{(A+H)^2+a^2-A^2}}
\frac1r\left[\frac{r^2}{r^2-a^2+A^2}-\frac{r^2-a^2+A^2}{r^2}\right]\,dr.}
$$

All endpoints and coefficients here depend only on $a$ and the specified material and reference geometry. This is the required implicit [pressure](../../../../pressure-split.md)–radius relation for [inflation and extension of an incompressible tube](../../../../inflation-and-extension-of-an-incompressible-tube.md) with unit axial stretch. In particular $a=A$ gives zero integrand and $P=0$. Once an admissible root is selected, the radial [stress](../../../../stress.md) follows by integrating from the outer face, $t_r(r)=-\int_r^b(dt_r/ds)\,ds$, and the remaining [stress](../../../../stress.md) components follow from the [constitutive equation](../../../../constitutive-equation.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
