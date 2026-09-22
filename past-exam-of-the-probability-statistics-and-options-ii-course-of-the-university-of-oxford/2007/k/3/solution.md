<h1 id="k/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Orient $C$ counterclockwise around the solid body and let $\mathbf n$ point from the solid into the fluid. The [pressure](../../../../pressure-split.md) [force](../../../../force-split.md) is $-\int_Cp\mathbf n\,ds$. Since $\mathbf n\,ds=(dy,-dx)$,

$$
F_x-iF_y=-i\oint_Cp\,d\overline z.
$$

For steady [irrotational flow](../../../../irrotational-flow.md), [Bernoulli's equation](../../../../bernoulli-equation.md) gives $p=p_0-\rho|w'|^2/2$. The constant term integrates to zero. The boundary is a [streamline](../../../../streamline.md), so $dw=w'\,dz$ is real there, giving $w'\,dz=\overline{w'}\,d\overline z$. Therefore

$$
F_x-iF_y=\frac{i\rho}{2}\oint_C|w'|^2\,d\overline z
=\frac{i\rho}{2}\oint_C(w')^2\,dz,
$$

which is [Blasius force theorem](../../../../blasius-force-theorem.md) with the specified orientation.

The prescribed [stream function](../../../../stream-function.md) is the imaginary part of $w_0(z)=\alpha(z-c)^3$. The zero-circulation solution from the [Milne-Thomson circle theorem](../../../../milne-thomson-circle-theorem.md) is

$$
w(z)=w_0(z)+\overline{w_0(a^2/\overline z)}
=\alpha\bigl[(z-c)^3+(a^2/z-c)^3\bigr].
$$

On $|z|=a$ the two terms are conjugates, so the boundary [stream function](../../../../stream-function.md) is constant. The added term has no singularities in the exterior and does not change the prescribed growing far-field part. Additive constants are immaterial.

Differentiating gives

$$
w'=3\alpha\bigl[z^2-2cz+c^2-c^2a^2z^{-2}+2ca^4z^{-3}-a^6z^{-4}\bigr].
$$

The coefficient of $z^{-1}$ in $(w')^2$ is $36\alpha^2ca^2(a^2+c^2)$. The [residue theorem](../../../../residue-theorem.md) and [Blasius force theorem](../../../../blasius-force-theorem.md) give

$$
\boxed{F_x=-36\pi\rho\alpha^2ca^2(a^2+c^2),\qquad F_y=0.}
$$

The zero-circulation convention is relevant: if an independently imposed [circulation](../../../../circulation-physics.md) $\Gamma$ is allowed, adding $\Gamma\log z/(2\pi i)$ changes $F_y$ to $-3\rho\alpha\Gamma c^2$. Thus the claimed zero transverse [force](../../../../force-split.md) belongs to the standard circle-theorem construction, or to a single-valued exterior [complex potential of a two-dimensional potential flow](../../../../complex-potential-of-a-two-dimensional-potential-flow.md), which excludes that extra circulation.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [K](../../k.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
