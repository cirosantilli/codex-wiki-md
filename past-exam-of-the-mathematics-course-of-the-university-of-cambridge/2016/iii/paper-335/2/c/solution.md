<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Seeking a [least-squares solution of a linear inverse problem](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) for the [acoustic inverse source problem](../../../../../../acoustic-inverse-source-problem.md) means minimizing $\|TQ-f_\infty\|^2$. **Its [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md) is**

$$
\boxed{T^*TQ=T^*f_\infty.}
$$

For compatible data, the formal minimum-norm solution can be written with the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md):

$$
\boxed{Q^\dagger=T^\dagger f_\infty
=\left[(T^*T)|_{(\ker T)^\perp}\right]^{-1}T^*f_\infty,\qquad
Q=Q^\dagger+h,\quad h\in\ker T.}
$$

The inverse in this expression is defined on the range of the restricted operator, not as a bounded everywhere-defined inverse. The unrestricted expression $(T^*T)^{-1}T^*f_\infty$ is only formal because $T$ has a nontrivial [kernel of a linear map](../../../../../../kernel-of-a-linear-map.md).

The [normal kernel of the source-to-far-field operator](../../../../../../normal-kernel-of-the-source-to-far-field-operator.md) can be computed explicitly:

$$
(T^*TQ)(\mathbf r)=\frac1{16\pi^2}\int_AQ(\mathbf r')
\left[\int_{S_1}e^{ik\boldsymbol\theta\cdot(\mathbf r-\mathbf r')}\,dS(\boldsymbol\theta)\right]d^3\mathbf r'
=\frac1{4\pi}\int_A\frac{\sin(k|\mathbf r-\mathbf r'|)}{k|\mathbf r-\mathbf r'|}Q(\mathbf r')\,d^3\mathbf r'.
$$

The quotient is $1$ at coincidence. This smooth kernel already exhibits the loss of information.

There are two distinct causes of [ill-posedness](../../../../../../ill-posed-problem.md). First, a [fixed-frequency nonradiating source](../../../../../../fixed-frequency-nonradiating-source.md) gives exact nonuniqueness. For any $\chi\in C_c^\infty(A)$, put

$$
Q_\chi=(\Delta+k^2)\chi.
$$

The outgoing solution is $\psi=\chi$, which vanishes outside $A$, so $TQ_\chi=0$. Equivalently, integration by parts in the [source-to-far-field operator at fixed frequency](../../../../../../source-to-far-field-operator-at-fixed-frequency.md) gives

$$
\int_A e^{-ik\boldsymbol\theta\cdot\mathbf r}(\Delta+k^2)\chi(\mathbf r)\,d^3\mathbf r=0,
$$

since the exponential solves the homogeneous [Helmholtz equation](../../../../../../helmholtz-equation.md) and the boundary terms vanish. This provides an infinite-dimensional family of invisible sources. Single-frequency data determine only the spherical restriction of a three-dimensional [Fourier transform](../../../../../../fourier-transform.md).

Second, the [compact operator](../../../../../../compact-operator-split.md) $T$ has arbitrarily small nonzero [singular values](../../../../../../singular-value.md). To see that its rank is infinite, choose a source $Q_{\ell m}(r\boldsymbol\eta)=q_\ell(r)Y_\ell^m(\boldsymbol\eta)$, with a [spherical harmonic](../../../../../../spherical-harmonic.md) $Y_\ell^m$. The plane-wave angular integral gives

$$
(TQ_{\ell m})(\boldsymbol\theta)=-(-i)^\ell Y_\ell^m(\boldsymbol\theta)\int_0^{r_0}q_\ell(r)j_\ell(kr)r^2\,dr.
$$

The [Spherical Bessel function](../../../../../../spherical-bessel-function.md) $j_\ell(kr)$ is not identically zero, so choose $q_\ell(r)=j_\ell(kr)$ to obtain a nonzero far-field coefficient for every $\ell$. The mutually orthogonal angular modes prove infinite rank. The inverse on $(\ker T)^\perp$ is therefore unbounded, and division by these small [singular values](../../../../../../singular-value.md) amplifies noise. Its range is not closed; arbitrary noisy $L^2(S_1)$ data need not be the [far-field pattern](../../../../../../far-field-pattern.md) of a source, and a [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) need not exist without [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md). For example, [Tikhonov regularization](../../../../../../tikhonov-regularization.md) gives $(T^*T+\lambda I)^{-1}T^*f^\delta_\infty$. It stabilizes the recovered visible component but cannot identify the missing [fixed-frequency nonradiating source](../../../../../../fixed-frequency-nonradiating-source.md) component.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
