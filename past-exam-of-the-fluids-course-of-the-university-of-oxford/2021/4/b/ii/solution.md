<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Taking the imaginary part of the [complex potential](../../../../../complex-potential-of-a-two-dimensional-potential-flow.md) gives the [streamfunction](../../../../../stream-function.md)

$$
\boxed{\psi=\beta[(x^2-y^2)\sin\alpha+2xy\cos\alpha]
=\beta r^2\sin(2\theta+\alpha).}
$$

The corresponding [velocity field](../../../../../velocity-field.md) is

$$
\begin{pmatrix}v_x\\v_y\end{pmatrix}
=2\beta
\begin{pmatrix}\cos\alpha&-\sin\alpha\\-\sin\alpha&-\cos\alpha\end{pmatrix}
\begin{pmatrix}x\\y\end{pmatrix}.
$$

Put $\zeta=z e^{i\alpha/2}=\xi+i\eta$. Then $w=\beta\zeta^2$ and $\psi=2\beta\xi\eta$. Thus the [streamlines](../../../../../streamline.md) are the previous rectangular [hyperbolas](../../../../../hyperbola.md) rotated clockwise by $\alpha/2$. Their separatrices have angles $\theta=-\alpha/2+n\pi/2$; the extension axis is $\theta=-\alpha/2$ and the compression axis is perpendicular to it. The middle panel of the figure shows this rotation.

For pure [advection](../../../../../advection.md), a marked [fluid element](../../../../../fluid-element.md) obeys

$$
\dot\xi=2\beta\xi,\qquad \dot\eta=-2\beta\eta,
\qquad
\xi(t)=e^{2\beta t}\xi(0),\quad \eta(t)=e^{-2\beta t}\eta(0).
$$

Consequently the dye circle becomes an [ellipse](../../../../../ellipse.md) with semiaxes $Re^{2\beta t}$ and $Re^{-2\beta t}$. Its [area](../../../../../surface-area.md) is

$$
\boxed{\mathcal A(t)=\pi(Re^{2\beta t})(Re^{-2\beta t})=\pi R^2.}
$$

Stretching in one principal direction exactly compensates compression in the other. Equivalently the flow-map [Jacobian determinant](../../../../../jacobian-determinant.md) is one, as required by [incompressibility](../../../../../incompressible-flow.md). Negligible [diffusion](../../../../../diffusion.md) is needed to regard the sharp dye boundary as a [material curve](../../../../../material-curve.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the fluids course of the University of Oxford](../../../../split.md)
6. [Fluids course of the University of Oxford](../../../../../fluids-course-of-the-university-of-oxford.md)
7. [Year 3 of the physics course of the University of Oxford](../../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
