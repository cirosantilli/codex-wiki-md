<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the discrete norm $\|U\|_h^2=h\sum_{m=1}^N|U_m|^2$, with periodic indices. Two independent arguments prove uniform [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md).

For [Fourier stability analysis](../../../../../../fourier-stability-analysis.md), a [discrete Fourier mode](../../../../../../discrete-fourier-mode.md) $U_m(t)=\widehat U_k(t)e^{im\theta_k}$ with $\theta_k=2\pi k/N$ has semidiscrete eigenvalue

$$
\lambda_h(\theta)=-\frac4{h^2}\sin^2(\theta/2)+i\frac\alpha h\sin\theta.
$$

Its real part is nonpositive, so $|\widehat U_k(t)|\leq|\widehat U_k(0)|$. The unitary [discrete Fourier transform](../../../../../../discrete-fourier-transform.md) and [discrete Parseval identity](../../../../../../discrete-parseval-identity.md) then give $\|U(t)\|_h\leq\|U(0)\|_h$ for every $N$, $t\geq0$ and fixed real $\alpha$.

For the [energy method](../../../../../../energy-method.md), denote the centered first difference by $D_0$ and the forward difference by $D_+$. Periodic [discrete summation by parts](../../../../../../discrete-summation-by-parts.md) makes $D_0$ skew-adjoint and gives $\langle U,D_{xx}U\rangle_h=-\|D_+U\|_h^2$. Therefore

$$
\boxed{\frac d{dt}\|U(t)\|_h^2
=2\operatorname{Re}\langle U,D_{xx}U+\alpha D_0U\rangle_h
=-2\|D_+U\|_h^2\leq0.}
$$

The constant mode is preserved rather than strictly damped. Both proofs apply equally to differences of two solutions. **The semidiscretization is contractive in the discrete L2 norm.** A later choice of a time integrator would require its own stability analysis; no time-step condition is needed for this continuous-time result.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [3](../../3.md)
3. [Section I](../../section-i.md)
4. [Paper 69](../../../paper-69-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
