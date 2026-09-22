<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

Using $\rho=\varepsilon_0\nabla\cdot E$, $E=-\nabla\phi$, integration by parts, and $\phi=0$ on the boundary gives

$$
U=\frac{\varepsilon_0}{2}\int_V|E|^2\,d^3x.
$$

Put $C=q/(4\pi\varepsilon_0)$. [Gauss's law](../../../../../gauss-s-law.md) gives the radial field

$$
E_r=\begin{cases}0,&r<R,\\C/r^2,&R<r<2R,\\-C/r^2,&2R<r<3R,\\0,&r>3R.\end{cases}
$$

Taking zero potential outside,

$$
\phi=\begin{cases}C/(3R),&r<R,\\C(1/r-2/(3R)),&R<r<2R,\\C(1/(3R)-1/r),&2R<r<3R,\\0,&r>3R.\end{cases}
$$

The charge formula gives

$$
U=\frac12\sum_iQ_i\phi(r_i)=\frac{q^2}{12\pi\varepsilon_0R}.
$$

The field formula gives the same result after integrating $4\pi r^2E_r^2$ over the two nonzero annuli.

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
