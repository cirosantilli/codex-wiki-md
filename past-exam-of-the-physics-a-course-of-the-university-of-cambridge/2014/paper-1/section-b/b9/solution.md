<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

Use $[x,p]=i\hbar$. Acting on a smooth test [wavefunction](../../../../../wave-function-split.md), $[f(x),p]\psi=f(-i\hbar\psi')+i\hbar(f\psi)'=i\hbar f'\psi$. Take $f$ real and use the [self-adjoint operator](../../../../../self-adjoint-operator.md) domain with vanishing integration-by-parts boundary terms. Writing $Q=p-if$ gives

$$
H=\frac{Q^\dagger Q}{2m}=\frac{p^2+f^2-\hbar f'}{2m},
\qquad\boxed{V(x)=\frac{f(x)^2-\hbar f'(x)}{2m}.}
$$

The [energy](../../../../../energy-split.md) form is $\langle\psi,H\psi\rangle=\|Q\psi\|^2/(2m)\ge0$, so every normalizable [energy eigenstate](../../../../../energy-eigenstate.md) has $E\ge0$. If a normalizable zero-energy state exists, its nonnegative norm must vanish, $Q\psi_0=0$. Hence

$$
\hbar\psi_0'+f\psi_0=0,\qquad
\boxed{\psi_0(x)=N\exp\left[-\frac1\hbar\int_0^xf(t)dt\right].}
$$

Zero [energy](../../../../../energy-split.md) is an additional existence assumption, not a consequence of factorization alone.

For $\psi_1=Q^\dagger\psi_0$, the [commutator](../../../../../commutator.md) $[Q,Q^\dagger]=2\hbar f'$ gives

$$
H\psi_1=\frac\hbar m Q^\dagger(f'\psi_0)
=-\frac{i\hbar^2}{m}f''\psi_0+\frac\hbar m f'\psi_1.
$$

Thus **$\alpha(x)=-i\hbar^2f''(x)/m$ and $\beta(x)=\hbar f'(x)/m$** in the requested relation. Generally these are multiplication functions, not constant coefficients, and $\psi_1$ is not automatically an [energy eigenstate](../../../../../energy-eigenstate.md).

If $f(x)=cx^n+\cdots$, its integral has leading term $cx^{n+1}/(n+1)$. Decay at both infinities on the full real line requires **odd $n$ and positive [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $c$**. Odd degree alone is not sufficient. For $f=kx$ take $k=m\omega>0$. Then $H=H_{\rm SHO}-\hbar\omega/2$, $\alpha=0$ and $\beta=\hbar\omega$. After normalization and removal of an irrelevant phase,

$$
\boxed{\psi_0=\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}e^{-m\omega x^2/(2\hbar)},\quad
\psi_1=\sqrt{\frac{2m\omega}{\hbar}}\,x\psi_0,\quad
E_0^{\rm SHO}=\frac12\hbar\omega,\quad E_1^{\rm SHO}=\frac32\hbar\omega.}
$$

The corresponding factorized-Hamiltonian energies are zero and $\hbar\omega$; the constant shift must be restored for the stated oscillator [Hamiltonian](../../../../../hamiltonian.md).

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
