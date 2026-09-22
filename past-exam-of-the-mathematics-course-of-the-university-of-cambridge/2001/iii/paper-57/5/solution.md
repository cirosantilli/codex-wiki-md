<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $S$ be the periodic forward-shift matrix, $(Su)_m=u_{m+1}$ with indices modulo $M$. The semidiscrete operator is

$$
u'=h^{-1}Au,\qquad A=-\frac32I+2S-\frac12S^2,\qquad h=\Delta x.
$$

For $\omega_\ell=e^{2\pi i\ell/M}$, $\ell=0,\ldots,M-1$, the vector $v^{(\ell)}=(1,\omega_\ell,\ldots,\omega_\ell^{M-1})^T$ satisfies $Sv^{(\ell)}=\omega_\ell v^{(\ell)}$. These vectors divided by $\sqrt M$ form the unitary [discrete Fourier transform](../../../../../discrete-fourier-transform.md) basis. Hence the normal matrix $A$ has [eigenvalues](../../../../../eigenvalue.md)

$$
\lambda_\ell=-\frac32+2e^{i\theta_\ell}-\frac12e^{2i\theta_\ell},\qquad
\operatorname{Re}\lambda_\ell=-\frac32+2\cos\theta_\ell-\frac12\cos2\theta_\ell=-(1-\cos\theta_\ell)^2\le0.
$$

Every Fourier coefficient is multiplied by $e^{t\lambda_\ell/h}$ of modulus at most one. [Parseval's identity](../../../../../parseval-identity.md) therefore proves

$$
\boxed{\|u(t)\|_{2,h}\le\|u(0)\|_{2,h},\qquad \|u\|_{2,h}^2=h\sum_{m=1}^M|u_m|^2.}
$$

The same estimate holds for differences of solutions and is uniform in the mesh. This is the required semidiscrete [stability of a numerical method](../../../../../stability-of-a-numerical-method.md). The mean mode has eigenvalue zero and is conserved, consistently with periodic advection.

One can also verify the energy estimate without diagonalization. Since $S^*=S^{-1}$,

$$
A+A^*=-\frac12(2I-S-S^*)^2,qquad
\frac d{dt}\|u\|_2^2=-\frac1{2h}\|(2I-S-S^*)u\|_2^2\le0.
$$

The [dissipative second-order forward advection semidiscretization](../../../../../dissipative-second-order-forward-advection-semidiscretization.md) thus damps nonconstant modes rather than amplifying them. This does not assert stability of an arbitrary further time-stepping method; its [absolute stability](../../../../../linear-stability-domain.md) region must contain the scaled eigenvalues. No nonnegativity condition on the periodic boundary value is needed: the printed trailing $t\ge0$ specifies the time range.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
