<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a normalized state and a [self-adjoint operator](../../../../self-adjoint-operator.md), the [expectation value](../../../../expectation-value.md) and dispersion are

$$
\boxed{\langle A\rangle_\psi=\langle\psi|A\psi\rangle,\qquad
\Delta_\psi(A)=\sqrt{\langle A^2\rangle_\psi-\langle A\rangle_\psi^2}.}
$$

Use the physics convention that the [inner product](../../../../inner-product-split.md) is conjugate-linear in its first argument, and assume the displayed products and second moments are defined. Self-adjointness gives $\overline{\langle\psi|A\psi\rangle}=\langle A\psi|\psi\rangle=\langle\psi|A\psi\rangle$, so the expectation is real. Moreover

$$
\Delta_\psi(A)^2=\|(A-\langle A\rangle_\psi)\psi\|^2.
$$

It vanishes exactly when $\psi$ is an eigenstate, with [eigenvalue](../../../../eigenvalue.md) its expectation.

The product rule gives $XPf=-i\hbar xf'$ and $PXf=-i\hbar(f+xf')$, hence $\boxed{[X,P]f=i\hbar f}$ on their common differentiable domain. For general operators, put $z=\langle A\psi|B\psi\rangle$. Then

$$
\langle[A,B]\rangle=z-\overline z=2i\operatorname{Im}z=i\langle C\rangle.
$$

The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) yields

$$
\boxed{\langle A^2\rangle\langle B^2\rangle
\geq|z|^2\geq(\operatorname{Im}z)^2=\frac14\langle C\rangle^2.}
$$

Apply this to centered position and [momentum operators](../../../../momentum-operator.md), whose [commutator](../../../../commutator.md) is unchanged. Their squared [norms](../../../../norm.md) are the [variances](../../../../variance-split.md), giving

$$
\boxed{\Delta P\,\Delta X\geq\hbar/2.}
$$

Equality requires both proportionality in Cauchy-Schwarz and a purely imaginary [inner product](../../../../inner-product-split.md). Thus for real means $x_0,p_0$,

$$
(P-p_0)\psi=i\gamma(X-x_0)\psi
$$

with real $\gamma$. Solving this first-order equation gives

$$
\psi(x)=N\exp\left[-\frac{\gamma(x-x_0)^2}{2\hbar}+\frac{ip_0x}{\hbar}\right].
$$

Normalizability on the real line forces $\gamma>0$. Writing $\sigma^2=\hbar/(2\gamma)$, all normalized equality states are therefore

$$
\boxed{\psi(x)=\frac{e^{i\phi}}{(2\pi\sigma^2)^{1/4}}
\exp\left[-\frac{(x-x_0)^2}{4\sigma^2}+\frac{ip_0x}{\hbar}\right],
\quad x_0,p_0,\phi\in\mathbb R,\quad\sigma>0.}
$$

They have $\Delta X=\sigma$ and $\Delta P=\hbar/(2\sigma)$. A nonconstant quadratic phase would increase the product, so the full family here has a real positive Gaussian width and only a linear spatial phase.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
