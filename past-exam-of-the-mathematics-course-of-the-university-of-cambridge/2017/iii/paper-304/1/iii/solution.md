<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use a real [orthonormal basis](../../../../../../orthonormal-basis.md) of [Fourier modes](../../../../../../fourier-mode.md) on the time circle:

$$
x_N(\tau)=\frac{q_0}{\sqrt\beta}+\sqrt{\frac2\beta}\sum_{r=1}^N\left[q_r\cos(\nu_r\tau)+s_r\sin(\nu_r\tau)\right],\qquad\nu_r=\frac{2\pi r}{\beta}.
$$

The [eigenvalue](../../../../../../eigenvalue.md) of $L_\omega$ on the constant mode is $\omega^2$, and each sine/cosine pair has [eigenvalue](../../../../../../eigenvalue.md) $\omega^2+\nu_r^2$. Retaining these modes gives

$$
S_{E,N}=\frac12\omega^2q_0^2+\frac12\sum_{r=1}^N(\omega^2+\nu_r^2)(q_r^2+s_r^2),\qquad
\mathcal D_Nx=C_N\,dq_0\prod_{r=1}^Ndq_r\,ds_r,
$$

where $C_N$ can depend on $N,\beta$ but is independent of $\omega$. Each real [Gaussian integral](../../../../../../gaussian-integral.md) contributes $\sqrt{2\pi/\lambda_r}$. Consequently the [Fourier-cutoff oscillator functional determinant](../../../../../../fourier-cutoff-oscillator-functional-determinant.md) is

$$
\boxed{\mathcal Z_N=\frac{A_N}{\omega}\prod_{r=1}^N(\omega^2+\nu_r^2)^{-1},\qquad A_N=C_N(2\pi)^{N+1/2}.}
$$

A spectral cutoff between successive [eigenvalue](../../../../../../eigenvalue.md) pairs selects precisely this finite subspace. In comparing two frequencies, the displayed regularization keeps the same number of modes $N$; holding an absolute spectral threshold fixed need not give the same $N$ at finite cutoff.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
