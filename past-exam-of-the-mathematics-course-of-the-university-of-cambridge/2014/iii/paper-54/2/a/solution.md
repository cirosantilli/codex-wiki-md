<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [magnetic field](../../../../../../magnetic-field.md) satisfies $\nabla\cdot\mathbf B=0$. Expanding the [divergence](../../../../../../divergence.md) of its [Maxwell stress tensor](../../../../../../maxwell-stress-tensor.md) gives

$$
\partial_jM_{ij}=\frac1{\mu_0}\left(B_j\partial_jB_i-\frac12\partial_iB^2\right)=\frac{[(\nabla\times\mathbf B)\times\mathbf B]_i}{\mu_0}.
$$

For the [Newtonian gravitational field](../../../../../../newtonian-gravitational-field.md) $\mathbf g=-\nabla\Phi$, [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) gives $\partial_jg_j=-4\pi G\rho$, and the [gradient](../../../../../../gradient.md) representation gives $\partial_jg_i=\partial_ig_j$. Consequently

$$
\partial_j\left(g_ig_j-\frac12g^2\delta_{ij}\right)=g_i\partial_jg_j+g_j(\partial_jg_i-\partial_ig_j)=-4\pi G\rho g_i.
$$

The negative of the [Newtonian gravitational stress tensor](../../../../../../newtonian-gravitational-stress-tensor.md), in this force-stress convention, therefore supplies $\rho g_i$. Adding the [pressure](../../../../../../pressure.md) stress supplies $-\partial_ip$, so

$$
\boxed{\rho D_tu_i=\partial_jT_{ij},\qquad T_{ij}=-p\delta_{ij}-\frac{g_ig_j-g^2\delta_{ij}/2}{4\pi G}+\frac{B_iB_j-B^2\delta_{ij}/2}{\mu_0}.}
$$

Each summand is symmetric. Absence of external gravitational sources is needed to represent the full gravitational force by this self-gravitating stress.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
