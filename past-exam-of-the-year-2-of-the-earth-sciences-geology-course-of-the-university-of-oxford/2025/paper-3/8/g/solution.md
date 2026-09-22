<h1 id="8/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

At $t=0$, the displacement expansion is $f(x)=\sum_nA_n\sin(n\pi x/L)$. [Fourier orthogonality](../../../../../fourier-orthogonality.md) gives

$$
\boxed{A_n=\frac2L\int_0^Lf(x)\sin\frac{n\pi x}{L}\,dx.}
$$

Differentiating the modal solution at zero gives $g(x)=\sum_n\omega_nB_n\sin(n\pi x/L)$, so

$$
\boxed{B_n=\frac{2}{L\omega_n}\int_0^Lg(x)\sin\frac{n\pi x}{L}\,dx
=\frac{2}{cn\pi}\int_0^Lg(x)\sin\frac{n\pi x}{L}\,dx.}
$$

The factor $1/\omega_n$ is required because the derivative of $\sin(\omega_nt)$ at zero is $\omega_n$. The dimensions agree: $A_n$ and $B_n$ are displacements, while the sine coefficients of $g$ are velocities. These projections also establish uniqueness within the finite-energy solution class.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [8](../../8.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2025](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
