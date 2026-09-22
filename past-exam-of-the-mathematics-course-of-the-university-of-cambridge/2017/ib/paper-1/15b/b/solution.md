<h1 id="15b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [bound state](../../../../../../bound-state.md) has $E<0$ and $\kappa=\sqrt{-2mE}/\hbar>0$, since outside the [delta potentials](../../../../../../delta-potential.md) a square-integrable solution must decay exponentially. The [wavefunction](../../../../../../wave-function.md) is continuous at each delta: a jump would produce a delta derivative in $\psi''$ with no matching term in the equation. Integrating the [Time-independent Schrödinger equation](../../../../../../time-independent-schrodinger-equation.md) across either $x_0=\pm a$ gives

$$
\boxed{\psi(x_0^+)=\psi(x_0^-),\quad\psi'(x_0^+)-\psi'(x_0^-)=-\frac{2m\lambda}{\hbar^2}\psi(x_0)}.
$$

The symmetry of the [symmetric double-delta potential](../../../../../../symmetric-double-delta-potential.md) permits even and odd solutions. Up to a nonzero normalization factor, the even candidate is $\cosh(\kappa x)$ for $|x|\le a$, and $\cosh(\kappa a)e^{-\kappa(|x|-a)}$ outside. Its derivative jump at $a$ gives

$$
\kappa(1+\tanh\kappa a)=\frac{2m\lambda}{\hbar^2}.
$$

The odd candidate is $\sinh(\kappa x)$ inside and $\operatorname{sgn}(x)\sinh(\kappa a)e^{-\kappa(|x|-a)}$ outside. Its jump gives

$$
\kappa(1+\coth\kappa a)=\frac{2m\lambda}{\hbar^2}.
$$

Parity ensures the jump at $-a$ as well. Put $t=\kappa a$ and $L=2m\lambda a/\hbar^2$. The continuous strictly increasing function $t(1+\tanh t)$ ranges from $0$ to infinity, so there is exactly one even [bound state](../../../../../../bound-state.md) for every $L>0$. The continuous strictly increasing function $t(1+\coth t)$ ranges from $1$ to infinity, so the [odd bound state of a symmetric double-delta potential](../../../../../../odd-bound-state-of-a-symmetric-double-delta-potential.md) exists if and only if $L>1$. Strict increase follows from the allowed monotonicity facts plus the strictly increasing term $t$. Therefore

$$
\boxed{\text{even: every }\lambda>0;\qquad\text{odd: }\lambda>\frac{\hbar^2}{2ma}},\qquad E=-\frac{\hbar^2\kappa^2}{2m}.
$$

At equality the odd limiting solution has $\kappa=0$ and is not square integrable, so it is not a [bound state](../../../../../../bound-state.md). No nonnegative energy can supply another full-line square-integrable state, since its exterior solutions are oscillatory or affine.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15B](../../15b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
