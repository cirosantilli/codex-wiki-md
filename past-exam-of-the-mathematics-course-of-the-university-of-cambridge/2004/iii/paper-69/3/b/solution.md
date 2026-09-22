<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [method of lines](../../../../../../method-of-lines.md) in part (a), the [Fourier symbol](../../../../../../fourier-symbol-of-a-difference-operator.md) of the spatial operator is

$$
\lambda_h(\theta)=h^{-2}\left(-\frac52+\frac83\cos\theta-\frac16\cos2\theta\right)=-\frac4{h^2}\sin^2\frac\theta2\left(1+\frac13\sin^2\frac\theta2\right)\le0.
$$

Each [Fourier mode](../../../../../../fourier-mode.md) therefore evolves by $\widehat U(\theta,t)=e^{t\lambda_h(\theta)}\widehat U(\theta,0)$, whose multiplier has [modulus](../../../../../../modulus.md) at most one. The [discrete Parseval identity](../../../../../../discrete-parseval-identity.md) gives

$$
\boxed{\|U(t)\|_{\ell_h^2}\le\|U(0)\|_{\ell_h^2}},\qquad\|U\|_{\ell_h^2}^2=h\sum_{m\in\mathbb Z}|U_m|^2.
$$

Thus the [fourth-order centered second derivative](../../../../../../fourth-order-centered-second-derivative.md) gives an **unconditionally stable semidiscrete evolution in the [L2 norm](../../../../../../l2-norm.md)**. No time integration method has yet been chosen, so no time-step restriction belongs to this conclusion.

An arbitrary [L2 function](../../../../../../square-integrable-function.md) does not have well-defined point samples. For the stated initial data one may use [cell-average projection](../../../../../../cell-average-projection.md), $U_m(0)=h^{-1}\int_{x_m-h/2}^{x_m+h/2}u_0(x)\,dx$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $h\sum_m|U_m(0)|^2\le\|u_0\|_{L^2}^2$, providing a bounded initialization for the stability estimate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
