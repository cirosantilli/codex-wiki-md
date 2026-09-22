<h1 id="k3/solution">Solution</h1>

↑ **Parent:** [K3](../k3.md)

Orient $\partial B$ counterclockwise, and define positive [circulation](../../../circulation-physics.md) by that orientation. The outward normal from the body satisfies $n\,ds=(dy,-dx)$. Pressure acts inward, so

$$
F_x-iF_y=-\oint p(dy+i\,dx)=-i\oint p\,d\overline z.
$$

The steady [Bernoulli equation](../../../bernoulli-equation.md) for this constant-density irrotational flow is $p+\rho|v|^2/2=C$. The constant has zero [integral](../../../integral-split.md) around a closed curve. With [complex potential of a two-dimensional potential flow](../../../complex-potential-of-a-two-dimensional-potential-flow.md) $w=\phi+i\psi$, let $W=w'=u-iv$. The no-penetration condition makes the boundary a streamline, so $dw=Wdz$ is real along it. Thus $Wdz=\overline Wd\overline z$, and $|W|^2d\overline z=W^2dz$. Substitution proves **[Blasius force theorem](../../../blasius-force-theorem.md)**:

$$
\boxed{F_x-iF_y=\frac{i\rho}{2}\oint_{\partial B}(w'(z))^2\,dz.}
$$

At infinity the [Laurent expansion](../../../laurent-series.md) has the form

$$
W(z)=U-iV+\frac{\Gamma}{2\pi iz}+O(z^{-2}).
$$

There is no source term because the impermeable body has zero net flux. The circulation term follows from $\oint Wdz=\Gamma$. The coefficient of $z^{-1}$ in $W^2$ is $\Gamma(U-iV)/(\pi i)$. Analyticity in the fluid lets the body contour be enlarged to a large counterclockwise circle, so the [residue theorem](../../../residue-theorem.md) gives $\oint W^2dz=2\Gamma(U-iV)$. Hence

$$
\boxed{(F_x,F_y)=\rho\Gamma(V,-U).}
$$

Its component along $(U,V)$ is zero: **the drag is zero**. The lift magnitude is $\boxed{\rho|\Gamma|\sqrt{U^2+V^2}}$. With the stated positive counterclockwise circulation, the signed lift along the left normal $(-V,U)/\sqrt{U^2+V^2}$ is $-\rho\Gamma\sqrt{U^2+V^2}$. Reversing the circulation convention reverses this signed formula. This is the [Kutta–Joukowski theorem](../../../kutta-joukowski-theorem.md) with its orientation made explicit.

## ↑ Ancestors (11)

1. [K3](../k3.md)
2. [2013](../../2013-split.md)
3. [Past exam of the options II course of the University of Oxford](../../split.md)
4. [Options II course of the University of Oxford](../../../options-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
