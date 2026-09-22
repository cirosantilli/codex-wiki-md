<h1 id="k/k3/solution">Solution</h1>

↑ **Parent:** [K3](../k3.md)

Orient the body boundary counterclockwise. The outward normal from the body satisfies $n\,ds=(dy,-dx)$, so pressure gives

$$
F_x-iF_y=-i\oint_Cp\,d\bar z.
$$

For steady [irrotational flow](../../../../irrotational-flow.md), Bernoulli's equation makes $p+\rho|u|^2/2$ constant in the [connected](../../../../connected-space.md) fluid region. Its constant contribution integrates to zero. Write $q=w'=u-iv$. Impermeability says the velocity is tangent to the boundary, so $q\,dz=\bar q\,d\bar z$ there. Consequently

$$
F_x-iF_y=\frac{i\rho}2\oint_C|q|^2d\bar z=\boxed{\frac{i\rho}2\oint_Cq^2\,dz},
$$

which proves Blasius' theorem with this contour convention.

The background [stream function](../../../../stream-function.md) is the imaginary part of $w_0(z)=\alpha(z-c)^3$. Since its coefficients are real, the circle theorem gives

$$
\boxed{w(z)=\alpha\{(z-c)^3+(a^2/z-c)^3\}}.
$$

Its derivative is

$$
q=\alpha(3z^2-6cz+3c^2-3a^6z^{-4}+6ca^4z^{-3}-3c^2a^2z^{-2}).
$$

In $q^2$ the coefficient of $z^{-1}$ comes from the exponent pairs $(2,-3)$ and $(1,-2)$, including both orders. It is $36\alpha^2ca^4+36\alpha^2c^3a^2$. The [residue theorem](../../../../residue-theorem.md) then gives

$$
\boxed{F_x=-36\pi\rho\alpha^2ca^2(a^2+c^2),\qquad F_y=0}.
$$

The vanishing transverse force also agrees with [reflection](../../../../reflection-mathematics.md) symmetry about the real axis.

## ↑ Ancestors (12)

1. [K3](../k3.md)
2. [K](../../k.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
