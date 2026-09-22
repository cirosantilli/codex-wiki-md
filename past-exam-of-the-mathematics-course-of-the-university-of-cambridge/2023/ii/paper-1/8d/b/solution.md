<h1 id="8d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In Cartesian components,

$$
\frac{\partial L}{\partial\dot r_i}=m\dot r_i+qA_i
$$

and

$$
\frac d{dt}\frac{\partial L}{\partial\dot r_i}
=m\ddot r_i+q\partial_tA_i+q\dot r_j\partial_jA_i,
\qquad
\frac{\partial L}{\partial r_i}
=-q\partial_i\phi+q\dot r_j\partial_iA_j.
$$

The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) therefore gives

$$
m\ddot r_i
=q\left[-\partial_i\phi-\partial_tA_i
 +\dot r_j(\partial_iA_j-\partial_jA_i)\right].
$$

Using

$$
E=-\nabla\phi-\partial_tA,
\qquad B=\nabla\times A,
$$

and $[\dot r\times B]_i=\dot r_j(\partial_iA_j-\partial_jA_i)$, this becomes the [Lorentz force](../../../../../../lorentz-force.md)

$$
\boxed{m\ddot r=q(E+\dot r\times B)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8D](../../8d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
