<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Take the [normal vector](../../../normal-vector.md) to point outward from the box. The [divergence theorem](../../../divergence-theorem.md) changes the closed-surface [flux](../../../flux.md) into a [volume integral](../../../volume-integral.md). The [divergence](../../../divergence.md) is

$$
\nabla\cdot F=\pi\cos(\pi x)+3zy^2+2z.
$$

The first term integrates to zero in $x$, since $\int_{-1}^{2}\pi\cos(\pi x)\,dx=\sin2\pi-\sin(-\pi)=0$. Therefore

$$
\begin{aligned}
\iint_SF\cdot d\boldsymbol S
&=\int_{-1}^2\int_0^1\int_1^4z(3y^2+2)\,dz\,dy\,dx\\
&=3\left(\frac{4^2-1^2}{2}\right)\left(\int_0^1(3y^2+2)\,dy\right)\\
&=3\cdot\frac{15}{2}\cdot3.
\end{aligned}
$$

Hence

$$
\boxed{\iint_SF\cdot d\boldsymbol S=\frac{135}{2}.}
$$

A direct face check gives zero from the two $x$ faces, $45/2$ from the pair of $y$ faces, and $45$ from the pair of $z$ faces. This also checks the outward-orientation signs.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
