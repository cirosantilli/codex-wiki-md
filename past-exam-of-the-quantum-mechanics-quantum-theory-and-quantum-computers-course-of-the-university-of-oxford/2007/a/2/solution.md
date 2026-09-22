<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Inside the box, the [time-independent Schrödinger equation](../../../../time-independent-schrodinger-equation.md) is $-\hbar^2\Psi''/(2m)=E\Psi$. The zero endpoint values eliminate the cosine term and require $ka=n\pi$. There is no nonzero zero-[energy](../../../../energy-split.md) solution with both endpoints zero. [Normalization](../../../../normalization.md) uses $\int_0^a\sin^2(n\pi x/a)\,dx=a/2$, so

$$
\boxed{E_n=\frac{n^2\pi^2\hbar^2}{2ma^2},\qquad
\Psi_n(x)=\sqrt{\frac2a}\sin\frac{n\pi x}{a},\qquad n=1,2,\ldots.}
$$

Insert the expansion into $i\hbar\partial_t\psi=H\psi$ and take its [inner product](../../../../inner-product-split.md) with $\Psi_m$. [Orthonormality](../../../../orthonormal-set.md) gives $i\hbar\dot c_m=E_mc_m$ for each $m$, and conversely these equations make every expansion coefficient of the residual zero. Thus $c_n(t)=c_n(0)e^{-iE_nt/\hbar}$ in the usual Hilbert-space or strong-solution class appropriate to the expansion.

For the specified state,

$$
\boxed{\psi(t,x)=\frac35e^{-iE_3t/\hbar}\Psi_3(x)+\frac45e^{-iE_4t/\hbar}\Psi_4(x).}
$$

The modes are real, so the [interference](../../../../interference-wave-propagation.md) term is a cosine of the [energy](../../../../energy-split.md) difference. Writing $s_n=\sin(n\pi x/a)$,

$$
\boxed{|\psi(t,x)|^2=\frac2{25a}\left[9s_3^2+16s_4^2+24s_3s_4\cos\!\left(\frac{7\pi^2\hbar t}{2ma^2}\right)\right].}
$$

Its integral remains one because the cross term integrates to zero. The probabilities of the two [energy](../../../../energy-split.md) outcomes are fixed at $9/25$ and $16/25$, even though the position [probability density](../../../../probability-density.md) oscillates.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
