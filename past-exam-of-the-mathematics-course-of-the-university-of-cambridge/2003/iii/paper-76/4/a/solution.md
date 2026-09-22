<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the explicit printed width law $b(z)=\alpha z^2$. Its wetted area and hydrostatic pressure integral are

$$
A(h)=\int_0^h b(z)dz=\frac{\alpha h^3}{3},\qquad
\mathcal P(h)=g\int_0^h(h-z)b(z)dz=\frac{g\alpha h^4}{12}.
$$

Assuming hydrostatic pressure, a horizontal prismatic bed and cross-sectionally uniform velocity, [volume conservation](../../../../../../volume-conservation.md) and [momentum conservation](../../../../../../momentum-conservation.md) give the [prismatic-channel shallow water equations](../../../../../../prismatic-channel-shallow-water-equations.md)

$$
A_t+(Au)_x=0,\qquad (Au)_t+(Au^2+\mathcal P)_x=0.
$$

Equivalently,

$$
h_t+uh_x+\frac h3u_x=0,\qquad u_t+uu_x+gh_x=0.
$$

The coefficient matrix in variables $(h,u)$ is $\begin{pmatrix}u&h/3\\g&u\end{pmatrix}$. Its eigenvalues and the corresponding gravity-wave speed are

$$
\boxed{\lambda_\pm=\frac{dx}{dt}=u\pm c,\qquad c=\sqrt{\frac{gh}{3}}.}
$$

For $h>0$ these eigenvalues are distinct and real, establishing strict hyperbolicity in the [hyperbolic partial differential equation](../../../../../../hyperbolic-partial-differential-equation.md) sense. Since $dc/dh=c/(2h)$, substitution in the two equations shows

$$
\boxed{J_\pm=u\pm6c\text{ is constant along }\frac{dx}{dt}=u\pm c.}
$$

For example $(\partial_t+(u+c)\partial_x)(u+6c)=0$. This provides both the slopes and the conserved characteristic quantities. At a dry bed $h=0$, strict hyperbolicity degenerates and the front is interpreted as the limit from positive depth.

The descriptive word “parabolic” alone would normally suggest $b\propto\sqrt z$ and different coefficients. The explicit $z^2$ width in the PDF determines the calculation here; it must not be silently replaced by that other geometry.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
