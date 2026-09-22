<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For either [scalar field](../../../../../../scalar-field.md) $f$ with mass $m_f$, the supplied covariant equation in the [FLRW metric](../../../../../../friedmann-lemaitre-robertson-walker-metric.md) is the [Klein-Gordon equation](../../../../../../klein-gordon-equation.md)

$$
\ddot f+3H\dot f-a^{-2}\nabla^2f+m_f^2f=0.
$$

Since $\dot f=f'/a$, $\ddot f=(f''-\mathcal Hf')/a^2$ and $H=\mathcal H/a$, its **conformal-time form** is

$$
\boxed{\phi''+2\mathcal H\phi'-\nabla^2\phi+a^2m_\phi^2\phi=0,
\qquad
\chi''+2\mathcal H\chi'-\nabla^2\chi+a^2m_\chi^2\chi=0.}
$$

The homogeneous [scalar field](../../../../../../scalar-field.md) backgrounds satisfy the same equations without spatial derivatives. After subtracting them, let $\delta\phi=u/a$ and $\delta\chi=v/a$. The key derivatives are

$$
(u/a)'=\frac{u'-\mathcal Hu}{a},\qquad
(u/a)''=\frac{u''-2\mathcal Hu'+(\mathcal H^2-\mathcal H')u}{a}.
$$

Because $a''/a=\mathcal H'+\mathcal H^2$, the expansion-friction term cancels after this [canonical rescaling of a scalar cosmological perturbation](../../../../../../canonical-rescaling-of-a-scalar-cosmological-perturbation.md). The **fluctuation equations** are

$$
\boxed{u''-\nabla^2u+\left(a^2m_\phi^2-\frac{a''}a\right)u=0,
\qquad
v''-\nabla^2v+\left(a^2m_\chi^2-\frac{a''}a\right)v=0.}
$$

The quadratic potential has no mixed derivative, and the stipulated neglect of [metric perturbations](../../../../../../linearized-gravity.md) removes gravitational mixing. Thus these two rescaled fluctuations evolve independently in this approximation.

The given symmetric [Fourier transform](../../../../../../fourier-transform.md) convention sends $-\nabla^2$ to $k^2$, where $k=|\mathbf k|$. Hence the **Fourier-mode equations** are

$$
\boxed{u_{\mathbf k}''+\left(k^2+a^2m_\phi^2-\frac{a''}a\right)u_{\mathbf k}=0,
\qquad
v_{\mathbf k}''+\left(k^2+a^2m_\chi^2-\frac{a''}a\right)v_{\mathbf k}=0.}
$$

They are harmonic-oscillator equations with time-dependent squared frequencies; a negative effective squared frequency for a rescaled field does not itself imply growth of the physical field $v/a$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
