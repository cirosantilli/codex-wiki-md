<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\lambda=\tfrac12\sum_j(x_jdy_j-y_jdx_j)$ on $\mathbb C^3$, so $d\lambda=\omega_{st}$. On a projective line, work in the affine coordinate $w=\rho e^{i\theta}$ and lift it to the unit three-sphere by

$$
s(w)=\frac{(w,1)}{\sqrt{1+|w|^2}}.
$$

This sphere lies in a complex two-plane in $\mathbb C^3$. The defining reduction identity for the [Fubini-Study form](../../../../../../fubini-study-form.md) gives $\Omega=s^*\omega_{st}$ on this chart. Differentiating the lift, or using the fact that real radial rescaling contributes no imaginary part to $\bar z\,dz$, gives

$$
s^*\lambda=\frac12\frac{\rho^2}{1+\rho^2}\,d\theta,
\qquad
\Omega=\frac{\rho}{(1+\rho^2)^2}\,d\rho\wedge d\theta.
$$

The missing point at infinity has zero area, so

$$
\boxed{\int_H\Omega=2\pi\int_0^\infty\frac{\rho\,d\rho}{(1+\rho^2)^2}=\pi.}
$$

This normalization is important: it differs from conventions in which a projective line has area $1$ or $2\pi$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
