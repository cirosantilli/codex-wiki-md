<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The supplied positive free-space kernel satisfies $-\Delta H=\delta$, so use the same sign convention for the [Dirichlet Green function](../../../../../dirichlet-green-function.md). For an interior source $Q=(\xi,\eta,\zeta)$, require

$$
-\Delta_PG(P;Q)=\delta_Q(P),\qquad G=0\text{ on }x=0\text{ and }z=0,\qquad G(P;Q)\to0\text{ as }|P|\to\infty.
$$

Away from $Q$, the function is [harmonic](../../../../../harmonic-function.md), and $G-H$ is regular near $Q$. The [method of images](../../../../../method-of-images.md) reflects the source in each coordinate plane, reversing its sign on each reflection. Therefore

$$
\boxed{G(P;Q)=\frac1{4\pi}\sum_{i,j=0}^1\frac{(-1)^{i+j}}{\sqrt{(x-(-1)^i\xi)^2+(y-\eta)^2+(z-(-1)^j\zeta)^2}}}.
$$

On either face, the terms cancel in pairs. Only the original source lies in the domain, so the other three terms are [harmonic](../../../../../harmonic-function.md) there; the required singularity and decay also follow. This is the [Dirichlet Green function for a three-dimensional quarter-space](../../../../../dirichlet-green-function-for-a-three-dimensional-quarter-space.md). Using $\Delta G=\delta$ instead would change the sign of the kernel and the representation formula together, as in [sign conventions for a Dirichlet Green function](../../../../../sign-conventions-for-a-dirichlet-green-function.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the applied partial differential equations course of the University of Oxford](../../../../split.md)
6. [Applied partial differential equations course of the University of Oxford](../../../../../applied-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
