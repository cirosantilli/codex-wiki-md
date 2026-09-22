<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [complex velocity](../../../../complex-velocity.md) $q(z)=w'(z)=u-iv$. For this steady, constant-[mass density](../../../../density.md), [irrotational flow](../../../../irrotational-flow.md) with no [body force](../../../../body-force.md), the applicable [Bernoulli equation](../../../../bernoulli-equation.md) is

$$
p+\frac\rho2|q|^2=P_*,
$$

with a single constant $P_*$ throughout the connected regular fluid region. The body's impermeability makes the [velocity](../../../../velocity.md) tangent to $C$. Thus $q\,dz$ is real there, giving

$$
q\,dz=\bar q\,d\bar z,\qquad |q|^2d\bar z=q^2dz.
$$

The [complex force](../../../../complex-force.md) from part (a) is

$$
\begin{aligned}
F_x-iF_y
&=-i\oint_Cp\,d\bar z\\
&=\frac{i\rho}{2}\oint_C|q|^2d\bar z
=\frac{i\rho}{2}\oint_Cq^2dz,
\end{aligned}
$$

where the constant-$P_*$ term vanishes. This proves the [Blasius force theorem](../../../../blasius-force-theorem.md):

$$
\boxed{F_x-iF_y=\frac{i\rho}{2}\oint_C\left(w'(z)\right)^2dz.}
$$

For the moment, observe that

$$
z\,d\bar z=(x\,dx+y\,dy)+i(y\,dx-x\,dy).
$$

Therefore $M=\operatorname{Re}\oint_Cp\,z\,d\bar z$. The constant [pressure](../../../../pressure-split.md) contribution has zero real part, because $x\,dx+y\,dy=\tfrac12d(x^2+y^2)$. Substituting [Bernoulli's principle](../../../../bernoulli-s-principle.md) and the same tangency identity gives the [Blasius moment theorem](../../../../blasius-moment-theorem.md):

$$
\boxed{M=-\frac\rho2\operatorname{Re}\oint_Cz\left(w'(z)\right)^2dz.}
$$

The real-part operation is essential: $\oint z\,d\bar z$ itself need not vanish, but its real part does.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
