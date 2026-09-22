<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Consider a string element of equilibrium length $dx$. Its [mass](../../../../mass.md) is $\rho\,dx$, where $\rho$ is mass per unit length. Under the small-slope approximation, the [tension](../../../../tension.md) is approximately uniform and its transverse component at an endpoint is $T\,\partial y/\partial x$. The two endpoint [forces](../../../../force-split.md) have net transverse component

$$
T\left[\frac{\partial y}{\partial x}(x+dx,t)-\frac{\partial y}{\partial x}(x,t)\right]\simeq T\frac{\partial^2y}{\partial x^2}\,dx.
$$

[Newton's second law](../../../../newton-s-second-law.md) gives $\rho\,dx\,y_{tt}=T\,dx\,y_{xx}$. Cancelling the element length yields

$$
\boxed{\frac{\partial^2y}{\partial t^2}-c^2\frac{\partial^2y}{\partial x^2}=0,\qquad c=\sqrt{\frac{T}{\rho}}}.
$$

This is the one-dimensional [wave equation](../../../../wave-equation-split.md) for transverse displacement. Its derivation neglects gravity, bending stiffness and nonlinear changes in [tension](../../../../tension.md) and segment length; the given small slope makes those omissions consistent to first order in the displacement.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [11](../../11.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
