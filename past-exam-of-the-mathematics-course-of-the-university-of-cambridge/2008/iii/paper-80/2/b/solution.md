<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $h=\Delta x$, impose $u_0=u_{M+1}=0$, and use the discrete [inner product](../../../../../../inner-product.md) $\langle u,v\rangle_h=h\sum_{m=1}^M\overline u_m v_m$. Discrete [integration by parts](../../../../../../integration-by-parts.md) for the second difference gives

$$
\operatorname{Re}\left[h\sum_{m=1}^M\overline u_m
\frac{u_{m-1}-2u_m+u_{m+1}}{h^2}\right]
=-\frac1h\sum_{m=0}^M|u_{m+1}-u_m|^2.
$$

For the centered drift, reindexing with the zero endpoints gives

$$
\operatorname{Re}\sum_{m=1}^M\overline u_m(u_{m+1}-u_{m-1})=0,
$$

since the two sums are complex conjugates. This is the fact that [centered discrete advection is skew-adjoint](../../../../../../centered-discrete-advection-is-skew-adjoint.md). The semidiscrete [energy estimate](../../../../../../energy-estimate.md) is therefore

$$
\boxed{\frac12\frac d{dt}\|u\|_h^2
=-\frac1h\sum_{m=0}^M|u_{m+1}-u_m|^2\leq0.}
$$

The finite-dimensional linear system has a unique solution for all times, and **$\|u(t)\|_h\leq\|u(0)\|_h$**, uniformly in the mesh and in real $\kappa$. Differences of two semidiscrete solutions obey the same bound, which is the required stability.

One may also use the smallest [eigenvalue](../../../../../../eigenvalue.md) $\lambda_h=4h^{-2}\sin^2(\pi/[2(M+1)])$ of the negative second-difference operator to obtain $\|u(t)\|_h\leq e^{-\lambda_ht}\|u(0)\|_h$. This conclusion concerns the [method of lines](../../../../../../method-of-lines.md); a later choice of time integrator has its own stability conditions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
