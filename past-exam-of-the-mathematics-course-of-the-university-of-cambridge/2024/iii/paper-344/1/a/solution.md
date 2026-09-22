<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\phi(\mathbf r)=V^{-1/2}\sum_{\mathbf q}\phi_{\mathbf q}e^{i\mathbf q\cdot\mathbf r},
\qquad
\phi_{-\mathbf q}=\phi_{\mathbf q}^*.
$$

The zero mode vanishes because the [compositional order parameter](../../../../../../compositional-order-parameter.md) has zero spatial average. [Parseval identity](../../../../../../parseval-identity.md) and the [Fourier transform of a derivative](../../../../../../fourier-transform-of-a-derivative.md) turn the quadratic part of the dimensionless free energy into

$$
H_{\rm G}
=\frac12\sum_{\mathbf q}
\left(a+\kappa q^2+\gamma q^4\right)|\phi_{\mathbf q}|^2
=\sum_{\mathbf q}^{+}G(q)|\phi_{\mathbf q}|^2,
\qquad
G(q)=a+\kappa q^2+\gamma q^4.
$$

Here $\sum_{\mathbf q}^{+}$ is the [positive-wavevector sum for a real field](../../../../../../positive-wavevector-sum-for-a-real-field.md). Each independent complex amplitude has density proportional to $e^{-G(q)|\phi_{\mathbf q}|^2}$, so its elementary [Gaussian integral](../../../../../../gaussian-integral.md) gives the [static structure factor](../../../../../../static-structure-factor.md)

$$
S(q)=\langle|\phi_{\mathbf q}|^2\rangle=\frac1{G(q)}
$$

whenever $G(q)>0$.

The stationary points of the [Brazovskii model](../../../../../../brazovskii-model.md) kernel obey

$$
G'(q)=2q(\kappa+2\gamma q^2)=0.
$$

Because $\kappa<0<\gamma$, the nonzero minimum is the [nonzero-wavevector soft-mode sphere](../../../../../../nonzero-wavevector-soft-mode-sphere.md)

$$
q_0^2=-\frac{\kappa}{2\gamma}.
$$

At this [wavevector](../../../../../../wavevector.md),

$$
G(q_0)=a-\frac{\kappa^2}{4\gamma}.
$$

The first [Gaussian field theory](../../../../../../gaussian-field-theory.md) divergence therefore occurs at

$$
\boxed{a_c=\frac{\kappa^2}{4\gamma}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
