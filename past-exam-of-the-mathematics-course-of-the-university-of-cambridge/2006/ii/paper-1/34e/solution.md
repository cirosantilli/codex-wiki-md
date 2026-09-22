<h1 id="34e/solution">Solution</h1>

↑ **Parent:** [34E](../34e.md)

Use rationalized electromagnetic units with $c=1$ and electrostatic constant $1/(4\pi)$. The [four-potential](../../../../../electromagnetic-four-potential.md) $A^a=(\varphi,A_x,A_y,A_z)$ transforms by the same [matrix](../../../../../matrix.md) as the coordinates:

$$
\boxed{\varphi'=\gamma(\varphi-vA_x),\quad A_x'=\gamma(A_x-v\varphi),\quad A_y'=A_y,\quad A_z'=A_z.}
$$

Write $r=\sqrt{y^2+z^2}$ and $\mathbf e_r=(0,y,z)/r$. [Gauss's law](../../../../../gauss-s-law.md) for the line at rest gives $\mathbf E'=\sigma\mathbf e_r/(2\pi r)$, $\mathbf B'=0$. A suitable potential is $\varphi'=-\sigma\log(r/r_*)/(2\pi)$, $\mathbf A'=0$. The inverse [Lorentz transformation](../../../../../lorentz-transformation.md) gives $\varphi=\gamma\varphi'$, $A_x=\gamma v\varphi'$. The fields from $\mathbf E=-\nabla\varphi-\partial_t\mathbf A$ and $\mathbf B=\nabla\times\mathbf A$ are therefore

$$
\boxed{\mathbf E=\frac{\gamma\sigma}{2\pi r}\mathbf e_r,\qquad\mathbf B=\frac{\gamma v\sigma}{2\pi r}\mathbf e_x\times\mathbf e_r.}
$$

The sign agrees with a [line charge](../../../../../line-charge.md) moving in the positive $x$ direction: its density is $\gamma\sigma$ and its current $\gamma v\sigma$. In SI units insert $1/\epsilon_0$ in the electric expressions and replace $\mathbf B=\mathbf v\times\mathbf E$ by $\mathbf B=\mathbf v\times\mathbf E/c^2$.

The two invariants check explicitly:

$$
\mathbf E\cdot\mathbf B=0=\mathbf E'\cdot\mathbf B',\qquad E^2-B^2=\gamma^2(1-v^2)\frac{\sigma^2}{4\pi^2r^2}=E'^2-B'^2.
$$

For $|v|\ll1$, the [electric field](../../../../../electric-field.md) differs from the static field only at order $v^2$, while the [magnetic field](../../../../../magnetic-field.md) is of order $v$ and is the field of the moving line current. These fields are evaluated off the charged axis.

## ↑ Ancestors (10)

1. [34E](../34e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
