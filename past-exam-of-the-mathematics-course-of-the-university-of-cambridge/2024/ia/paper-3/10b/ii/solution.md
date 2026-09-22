<h1 id="10b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Close the surface with the unit disk $D$ in the plane $z=0$. Its outward normal is $-e_z$, but $F\cdot(-e_z)=-z^4=0$ there. Also

$$
\nabla\cdot F=2x-2y+4z^3.
$$

The $x$ and $y$ terms integrate to zero by symmetry. The [divergence theorem](../../../../../../divergence-theorem.md) therefore gives

$$
\begin{aligned}
\int_SF\cdot dS
&=\int_0^{2\pi}\int_0^1\int_0^{1-r^2}
4z^3r\,dz\,dr\,d\theta\\
&=2\pi\int_0^1r(1-r^2)^4\,dr
=\boxed{\frac\pi5}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10B](../../10b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
