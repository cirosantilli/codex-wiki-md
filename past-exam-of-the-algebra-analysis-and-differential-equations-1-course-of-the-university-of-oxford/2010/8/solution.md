<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Here a periodic solution must mean a nonconstant periodic orbit: constant equilibria are not excluded by the stated divergence hypothesis. Suppose such an orbit exists. Since the vector field is continuously differentiable, uniqueness for the [autonomous differential equation](../../../autonomous-system-mathematics.md) makes its trajectory a simple closed curve $C$, bounding a region $D$ by the [Jordan curve theorem](../../../jordan-curve-theorem.md). The [Green theorem](../../../green-theorem.md) gives

$$
\iint_D\left[\partial_x(\rho f)+\partial_y(\rho g)\right]dx\,dy
=\oint_C\rho f\,dy-\rho g\,dx.
$$

Along the orbit, $dx=fdt$ and $dy=gdt$, so the line integral is identically zero. Reversing orientation if necessary does not change this conclusion. The area integral is strictly positive because its continuous integrand is positive everywhere and $D$ has positive area. This contradiction proves the [Bendixson-Dulac criterion](../../../bendixson-dulac-theorem.md) in this case.

For the second-order equation set $y=x'$, giving $x'=y$, $y'=-y-\varepsilon y^3-\sin x$. Choose the [Dulac function](../../../dulac-function.md) $\rho=-1$. Then

$$
\partial_x(\rho f)+\partial_y(\rho g)=1+3\varepsilon y^2>0.
$$

Thus **there is no nonconstant periodic solution for $\varepsilon>0$**. The equilibria $x(t)=k\pi$ do remain solutions. As a direct check, the mechanical energy $H=y^2/2+1-\cos x$ obeys $H'=-y^2-\varepsilon y^4$, whose integral over a period could vanish only if $y\equiv0$.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2010](../../2010-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
