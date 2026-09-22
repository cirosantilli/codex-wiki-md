<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Orient $C$ counterclockwise around the body. For an arc element $ds$, the body-outward [unit normal vector](../../../../unit-normal.md) obeys $\mathbf n\,ds=(dy,-dx)$. The [pressure](../../../../pressure-split.md) acts normally into the body, so its [force per unit length](../../../../force-per-unit-length.md) in the suppressed third direction is

$$
d\mathbf F=-p\mathbf n\,ds=(-p\,dy,p\,dx).
$$

Integrating gives

$$
\boxed{F_x=-\oint_Cp\,dy,\qquad F_y=\oint_Cp\,dx.}
$$

Taking positive [torque](../../../../torque.md) to mean counterclockwise about the origin, the infinitesimal moment is $dM=x\,dF_y-y\,dF_x=p(x\,dx+y\,dy)$. Hence

$$
\boxed{M=\oint_Cp(x\,dx+y\,dy).}
$$

All three expressions are per unit span. They are the normal-[pressure](../../../../pressure-split.md) contributions assumed by the inviscid model; a viscous [traction](../../../../traction.md) would require extra terms. A constant [pressure](../../../../pressure-split.md) contributes zero net [force](../../../../force-split.md) and [torque](../../../../torque.md) on a closed body, since $\oint dx=\oint dy=\oint d(x^2+y^2)=0$.

## ↑ Ancestors (12)

1. [A](../a.md)
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
