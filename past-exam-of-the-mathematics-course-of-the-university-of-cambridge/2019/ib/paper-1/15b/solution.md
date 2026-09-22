<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

The [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md) for the one-dimensional [Quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md) is

$$
i\hbar\frac{\partial\Psi}{\partial t}
=\left(-\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}
+\frac12m\omega^2x^2\right)\Psi.
$$

A [stationary state](../../../../../stationary-state.md) has $\Psi(x,t)=\psi(x)e^{-iEt/\hbar}$, so cancellation of the common time factor gives

$$
-\frac{\hbar^2}{2m}\psi''+\frac12m\omega^2x^2\psi=E\psi.
$$

Set

$$
y=\sqrt{\frac{m\omega}{\hbar}}x,
\qquad
\epsilon=\frac{2E}{\hbar\omega}.
$$

The equation becomes

$$
\boxed{-\frac{d^2\psi}{dy^2}+y^2\psi=\epsilon\psi}.
$$

With $\psi=f(y)e^{-y^2/2}$,

$$
\psi''=\left[f''-2yf'+(y^2-1)f\right]e^{-y^2/2},
$$

and hence $f$ obeys the [Hermite differential equation](../../../../../hermite-differential-equation.md)

$$
\boxed{f''-2yf'+(\epsilon-1)f=0}.
$$

If $f$ is monic of degree $N$, the coefficient of $y^N$ in this equation is $\epsilon-1-2N$. It must vanish, so

$$
\boxed{\epsilon=2N+1,
\qquad E=\hbar\omega\left(N+\frac12\right)}.
$$

Writing $f=\sum_{k=0}^Na_ky^k$ gives the recurrence

$$
a_{k+2}=\frac{2(k-N)}{(k+2)(k+1)}a_k.
$$

The coefficient of $y^{N-1}$ first gives $a_{N-1}=0$, and the recurrence preserves parity. If $N$ is even, every odd coefficient vanishes, so $f$ is an [even function](../../../../../even-function.md). The Gaussian factor is also even; therefore the stationary state $\psi$ has even [parity](../../../../../parity.md).

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
