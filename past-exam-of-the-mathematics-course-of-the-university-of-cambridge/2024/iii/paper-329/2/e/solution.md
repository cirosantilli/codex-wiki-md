<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A vector fixed in space has [body-frame derivative of a space-fixed vector](../../../../../../body-frame-derivative-of-a-space-fixed-vector.md)

$$
\left(\frac{d\mathbf k}{dt}\right)_{\rm body}
=-\boldsymbol\Omega\times\mathbf k.
$$

Substitution of part (d) gives

$$
\boxed{
\frac d{dt}(k_x,k_y,k_z)
=\frac\gamma L
(k_xk_z,-k_yk_z,k_y^2-k_x^2)}.
$$

If $\boldsymbol\Omega$ is constant and nonzero, then $k_x$ and $k_y$ are constant and not both zero. Their evolution equations force $k_z=0$, and the last equation then gives $k_x^2=k_y^2$. Hence

$$
\boxed{\mathbf k\parallel(1,1,0)
\quad\text{or}\quad
\mathbf k\parallel(1,-1,0)}.
$$

For $\mathbf k=(1,1,0)$, both the translational velocity and the angular velocity are parallel to the fixed vertical force, with the latter oppositely directed. The body therefore falls on a straight vertical line while spinning steadily about that line. Its body $z$-axis remains horizontal, and its $x$- and $y$-axes remain at $45^\circ$ to the vertical.

For the initial condition $(1,0,0)$, symmetry preserves $k_y=0$. With $c=\gamma/L$ the exact body-frame solution is

$$
k_x=\operatorname{sech}(ct),
\qquad
k_z=-\tanh(ct).
$$

The body rotates about its $y$-axis, its fall path bends slightly because the horizontal and axial mobilities differ, and $\mathbf k\to(0,0,-1)$. Thus the body $z$-axis becomes vertical and the angular velocity tends to zero; asymptotically it falls without rotating.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
