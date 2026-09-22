<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $x_m=mh$ be a uniform periodic mesh, with indices interpreted modulo the number of nodes. Write the [finite element](../../../../../../finite-element.md) approximation as $u_h(x,t)=\sum_jU_j(t)\phi_j(x)$ using the [chapeau functions](../../../../../../piecewise-linear-hat-function.md). The [Galerkin method](../../../../../../galerkin-method.md) requires

$$
\int_0^1\partial_tu_h\,\phi_m\,dx=\int_0^1\partial_xu_h\,\phi_m\,dx.
$$

The [mass matrix](../../../../../../mass-matrix.md) has $M_{mm}=2h/3$ and $M_{m,m\pm1}=h/6$. The spatial [matrix](../../../../../../matrix.md) $C_{mj}=\int\phi_m\phi_j'$ has $C_{m,m+1}=1/2$ and $C_{m,m-1}=-1/2$, with zero diagonal. Therefore the semidiscrete equations are

$$
\boxed{\frac h6\left(\dot U_{m-1}+4\dot U_m+\dot U_{m+1}\right)=\frac12(U_{m+1}-U_{m-1}),}
$$

or equivalently $M\dot U=CU$. The coefficients come from integrating the products of the two overlapping [piecewise-linear hat functions](../../../../../../piecewise-linear-hat-function.md) on each interval; periodicity supplies the wraparound entries.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
