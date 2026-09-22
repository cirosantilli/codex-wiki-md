<h1 id="j/j1/solution">Solution</h1>

↑ **Parent:** [J1](../j1.md)

[Ampère's law](../../../../ampere-s-circuital-law.md) in magnetostatics is

$$
\oint_\Gamma B\cdot d\ell=\mu_0 I_S,\qquad I_S=\int_SJ\cdot n\,dS,
$$

with boundary and surface orientations related by the right-hand rule. Stokes' theorem gives the left side as $\int_S(\nabla\times B)\cdot n\,dS$, proving the integral law from the stated curl equation.

For a circular contour of radius $r$ about the axis, the left side is $2\pi rB_\theta$. For $r\le a$ the enclosed current is $Ir^2/a^2$; for $r\ge a$ it is $I$. Therefore

$$
\boxed{B(r)=\begin{cases}\dfrac{\mu_0 I r}{2\pi a^2}\,e_\theta,&0<r\le a,\\[2mm]\dfrac{\mu_0 I}{2\pi r}\,e_\theta,&r\ge a.\end{cases}}
$$

Both expressions agree at the boundary. At the axis the field is zero, interpreted by [continuity](../../../../continuous-function.md) even though the angular unit vector is undefined there.

## ↑ Ancestors (12)

1. [J1](../j1.md)
2. [J](../../j.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
