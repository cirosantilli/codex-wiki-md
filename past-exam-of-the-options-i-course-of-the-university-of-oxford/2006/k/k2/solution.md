<h1 id="k/k2/solution">Solution</h1>

↑ **Parent:** [K2](../k2.md)

Start from the uniform-flow [complex potential of a two-dimensional potential flow](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) $Uz$. [Milne-Thomson's circle theorem](../../../../milne-thomson-circle-theorem.md) adds the image doublet $Ua^2/z$, yielding constant [stream function](../../../../stream-function.md) on $|z|=a$. Add a [line vortex](../../../../line-vortex.md) with positive counterclockwise [circulation](../../../../circulation-physics.md) $\Gamma$:

$$
\boxed{w(z)=U\left(z+\frac{a^2}{z}\right)-\frac{i\Gamma}{2\pi}\log z}.
$$

Indeed, on $z=ae^{i\theta}$ the uniform-flow and doublet terms sum to the real number $2Ua\cos\theta$, while the vortex has imaginary part $-\Gamma\log a/(2\pi)$, also constant. Thus the cylinder is a [streamline](../../../../streamline.md) and satisfies the [impermeability condition](../../../../no-penetration-boundary-condition.md). The vortex velocity is $\Gamma/(2\pi r)$ in the counterclockwise direction. Although the potential is multivalued when $\Gamma\ne0$, its velocity is single-valued.

Differentiate and locate the coefficient of $z^{-1}$ in the square:

$$
w'=U-\frac{i\Gamma}{2\pi z}-\frac{Ua^2}{z^2},\qquad\operatorname{Res}_{z=0}(w')^2=-\frac{iU\Gamma}{\pi}.
$$

For the counterclockwise contour in the printed [Blasius force theorem](../../../../blasius-force-theorem.md), the [residue theorem](../../../../residue-theorem.md) gives $\oint_C(w')^2dz=2U\Gamma$. Consequently

$$
F_x-iF_y=i\rho U\Gamma,\qquad\boxed{F_x=0,\quad F_y=-\rho U\Gamma}.
$$

These are force components per unit cylinder length; with the stated [circulation](../../../../circulation-physics.md) convention the lift is downward for positive $U\Gamma$.

## ↑ Ancestors (12)

1. [K2](../k2.md)
2. [K](../../k.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
