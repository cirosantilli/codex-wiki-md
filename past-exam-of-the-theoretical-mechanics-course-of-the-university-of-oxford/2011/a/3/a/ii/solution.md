<h1 id="a/3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppress hats temporarily. Mass conservation between any two cross-sections, together with impermeability of both walls, makes their fluxes equal. Where the wall is differentiable, the same result follows locally by differentiating the [flux](../../../../../../flux.md) with a variable upper limit and using continuity gives

$$
Q'(x)=\int_0^{h(x)}u_x\,dz+u(x,h)h'=-\int_0^hw_z\,dz=-(w(x,h)-w(x,0))=0.
$$

Both the upper-limit term and the boundary velocities vanish by the wall conditions. Thus **the [flux](../../../../../../flux.md) is constant**. Since $p=p(x)$, integrate $u_{zz}=p'(x)$ twice and impose $u(0)=1$, $u(h)=0$:

$$
\boxed{u(x,z)=1-\frac zh+\frac{p'}2z(z-h).}
$$

Integrating across the gap gives $Q=h/2-p'h^3/12$. Restoring hats,

$$
\boxed{\frac{d\widehat p}{d\widehat x}=\frac{6(\widehat h-2Q)}{\widehat h^3},\qquad
\widehat p(-1)=\widehat p(1)=0.}
$$

The endpoint conditions are the specified equal reservoir pressures after subtracting $p_0$ and dividing by the [pressure](../../../../../../pressure-split.md) scale.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
