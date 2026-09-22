<h1 id="11/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a single [normal mode](../../../../normal-mode.md) $y_n=A_n\sin(k_nx)\cos(\omega_nt+\phi_n)$, the [kinetic energy](../../../../kinetic-energy.md) is the integral of $\tfrac12\rho y_t^2$. Using $\int_0^l\sin^2(k_nx)\,dx=l/2$ gives

$$
\boxed{K_n(t)=\frac{\rho l\omega_n^2A_n^2}{4}\sin^2(\omega_nt+\phi_n)}.
$$

The extra string length is $\int_0^l[\sqrt{1+y_x^2}-1]dx\simeq\tfrac12\int_0^l y_x^2dx$. Multiplying by [tension](../../../../tension.md) gives the quadratic [potential energy](../../../../potential-energy.md), so $\int_0^l\cos^2(k_nx)dx=l/2$ implies

$$
\boxed{U_n(t)=\frac{Tl k_n^2A_n^2}{4}\cos^2(\omega_nt+\phi_n)}.
$$

Since $\rho\omega_n^2=Tk_n^2$, the sum is time independent:

$$
\boxed{E_n=K_n+U_n=\frac{Tl k_n^2A_n^2}{4}=\frac{n^2\pi^2TA_n^2}{4l}}.
$$

For the released shape, $A_1=A$ and $A_2=A/2$, so

$$
\boxed{E_1=E_2=\frac{\pi^2TA^2}{4l},\qquad E_{\rm total}=\frac{\pi^2TA^2}{2l}}.
$$

The second mode's smaller displacement is offset by its doubled spatial [wavenumber](../../../../wavenumber.md) and [angular frequency](../../../../angular-frequency.md). [orthogonality](../../../../orthogonal-vectors.md) of distinct sine and cosine spatial modes eliminates cross terms in the integrated energies, so the total is their sum. Initially the [kinetic energy](../../../../kinetic-energy.md) is zero and all the [energy](../../../../energy-split.md) is stored in the string's deformation; during the motion the total remains constant.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [11](../../11.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
