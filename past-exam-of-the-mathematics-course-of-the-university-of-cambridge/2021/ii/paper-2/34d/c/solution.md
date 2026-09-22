<h1 id="34d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each discrete term satisfies

$$
\partial_t(c_n^2e^{-\kappa_nx})=8\kappa_n^3c_n^2e^{-\kappa_nx}
=-8\partial_x^3(c_n^2e^{-\kappa_nx}),
$$

and the same identity follows for the Fourier integral from $R_t=8ik^3R$. Hence

$$
F_t+8F_{xxx}=0.
$$

Apply $\partial_x^2-\partial_y^2-u(x,t)$ to the [Gelfand-Levitan-Marchenko equation](../../../../../../marchenko-equation.md). Differentiating under the integral and integrating the $z$ derivatives by parts, the boundary terms combine to $u=-2\partial_xK(x,x,t)$. The terms containing $F$ cancel, leaving

$$
\boxed{G(x,y,t)+\int_x^\infty G(x,z,t)F(z+y,t)\,dz=0}.
$$

Uniqueness of the Marchenko equation then also gives $G=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [34D](../../34d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
