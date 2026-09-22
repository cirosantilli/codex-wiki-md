<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Compare the [total differential](../../../../total-differential.md) $d\phi=\sum_i\partial_{u_i}\phi\,du_i$ with $d\phi=\nabla\phi\cdot d\mathbf r$ and $d\mathbf r=\sum_i h_i\mathbf e_i\,du_i$. The orthonormality of the coordinate basis gives the [gradient in orthogonal coordinates](../../../../gradient-in-orthogonal-coordinates.md):

$$
\boxed{\nabla\phi=\sum_{i=1}^3\frac{\mathbf e_i}{h_i}\partial_{u_i}\phi,\qquad \nabla u_i=\frac{\mathbf e_i}{h_i}.}
$$

To obtain the [curl](../../../../curl.md) without neglecting the variation of the basis vectors, write $\phi\mathbf e_1=(\phi h_1)\nabla u_1$. The curl of a gradient vanishes, and the product rule gives

$$
\nabla\times(\phi\mathbf e_1)=\nabla(\phi h_1)\times\nabla u_1=\frac{\mathbf e_2}{h_1h_3}\partial_{u_3}(\phi h_1)-\frac{\mathbf e_3}{h_1h_2}\partial_{u_2}(\phi h_1).
$$

Likewise $\nabla u_2\times\nabla u_3=\mathbf e_1/(h_2h_3)$ because the system is right-handed. This cross product has zero [divergence](../../../../divergence.md): $\nabla\cdot(\nabla u_2\times\nabla u_3)=\nabla u_3\cdot(\nabla\times\nabla u_2)-\nabla u_2\cdot(\nabla\times\nabla u_3)=0$. The divergence product rule applied to $(\phi h_2h_3)(\nabla u_2\times\nabla u_3)$ now gives

$$
\nabla\cdot(\phi\mathbf e_1)=\frac1{h_1h_2h_3}\partial_{u_1}(\phi h_2h_3).
$$

Cyclic permutation and linearity give the general component formulas described by [divergence and curl from orthogonal coordinate gradients](../../../../divergence-and-curl-from-orthogonal-coordinate-gradients.md):

$$
\boxed{\nabla\cdot\mathbf v=\frac{\partial_{u_1}(h_2h_3v_1)+\partial_{u_2}(h_3h_1v_2)+\partial_{u_3}(h_1h_2v_3)}{h_1h_2h_3},}
$$

and

$$
\boxed{\nabla\times\mathbf v=\frac{\mathbf e_1}{h_2h_3}[\partial_{u_2}(h_3v_3)-\partial_{u_3}(h_2v_2)]+\frac{\mathbf e_2}{h_3h_1}[\partial_{u_3}(h_1v_1)-\partial_{u_1}(h_3v_3)]+\frac{\mathbf e_3}{h_1h_2}[\partial_{u_1}(h_2v_2)-\partial_{u_2}(h_1v_1)].}
$$

In [cylindrical coordinates](../../../../cylindrical-coordinate-system.md), $(h_r,h_\theta,h_z)=(1,r,1)$. The specified field has no $z$ dependence or $z$ component, so

$$
\boxed{\nabla\times\mathbf v=\left[\frac1r\partial_r(r^4)-\frac1r\partial_\theta(\alpha\theta r^p)\right]\mathbf e_z=(4r^2-\alpha r^{p-1})\mathbf e_z.}
$$

It is an [irrotational vector field](../../../../irrotational-vector-field.md) for every $r>0$ exactly when $\boxed{p=3,\ \alpha=4}$. This statement is local to an angular coordinate chart: the component proportional to $\theta$ is not single-valued under $\theta\mapsto\theta+2\pi$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2004](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
