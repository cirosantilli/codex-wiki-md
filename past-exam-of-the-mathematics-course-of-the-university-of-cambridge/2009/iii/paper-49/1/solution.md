<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Substitution of the stationary ansatz into the [focusing nonlinear Schrodinger equation](../../../../../focusing-nonlinear-schrodinger-equation.md) gives the real [ordinary differential equation](../../../../../ordinary-differential-equation.md)

$$
Ef=-\frac12f''-f^3,\qquad f''+2Ef+2f^3=0.
$$

Multiply by $2f'$ and integrate to obtain the first integral

$$
(f')^2+2Ef^2+f^4=C.
$$

The finite [L2 norm](../../../../../l2-norm.md) forces the relevant orbit to approach $(f,f')=(0,0)$ and hence $C=0$. To justify this rather than assume pointwise decay, the conserved expression first bounds $f$ and $f'$, since $f^4+2Ef^2$ tends to infinity with $|f|$. Thus $f^2$ is uniformly continuous and integrable, and tends to zero at both ends. If $C>0$, then $|f'|$ would eventually be bounded away from zero with fixed sign, contradicting $f\to0$; $C<0$ is incompatible with $(f')^2=C-2Ef^2-f^4$ near zero. Therefore $C=0$ and $f'\to0$.

For $E\geq0$, the identity $(f')^2=-2Ef^2-f^4$ permits only $f=0$. For a nonzero localized profile put $\kappa=\sqrt{-2E}>0$. Then

$$
(f')^2=f^2(\kappa^2-f^2).
$$

A nonzero solution cannot cross zero, because at a zero it also has $f'=0$, and uniqueness of the [ordinary differential equation](../../../../../ordinary-differential-equation.md) would make it identically zero. Its sign is fixed, its maximum absolute value is $\kappa$, and separation on either side of that maximum gives

$$
\boxed{f(x)=\pm\kappa\operatorname{sech}(\kappa(x-X_0)),\qquad E=-\frac{\kappa^2}{2}.}
$$

Direct differentiation verifies the profile and its squared [L2 norm](../../../../../l2-norm.md) is $\int f^2dx=2\kappa$. The two signs can be incorporated into an arbitrary constant phase of the complex [bright soliton of the focusing nonlinear Schrödinger equation](../../../../../bright-soliton-of-the-focusing-nonlinear-schrodinger-equation.md).

For a [Galilean boost of a nonlinear Schrödinger soliton](../../../../../galilean-boost-of-a-nonlinear-schrodinger-soliton.md), define $\psi_u(x,t)=e^{i(ux-u^2t/2)}\psi_0(x-ut,t)$. Differentiating shows that the terms proportional to $u\partial_x\psi_0$ cancel between $i\partial_t$ and $-\partial_x^2/2$, as do the added $u^2/2$ terms. The cubic nonlinearity is unchanged because the multiplying phase has modulus one. Hence the boosted field solves the same equation. In particular,

$$
\boxed{\psi(x,t)=\kappa\operatorname{sech}(\kappa(x-ut-X_0))
\exp\left\{iux-i\left(\frac{u^2}{2}-\frac{\kappa^2}{2}\right)t+i\theta_0\right\},}
$$

whose centre follows $X(t)=ut+X_0$.

For the slowly varying external potential, use the [collective-coordinate effective Lagrangian](../../../../../collective-coordinate-effective-lagrangian-for-a-soliton.md) method: retain the localized free profile but let its centre, boost and overall phase vary with time, with its norm fixed. Substitute this finite-parameter ansatz into the field [Lagrangian](../../../../../lagrangian.md), integrate over space and derive the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) for the parameters. The potential contribution is the external potential averaged over the soliton's density; if it varies little across the profile, it is approximately its value at the centre times the conserved norm. This gives approximate particle-like centre motion while neglecting radiation and profile deformation. No solution of the full perturbed field equation is required for this approximation.

For the harmonic trap, keep the assumed trapped stationary profile $f(y)$, and put $y=x-X(t)$. Take $\Theta(x,t)=v(t)x+\gamma(t)-Et$. Substituting $e^{i\Theta}f(y)$, the imaginary terms are $-i\dot Xf'$ on the left and $-ivf'$ on the right, so choose $v=\dot X$. Using the profile equation, the remaining real equation is

$$
-\Theta_tf=\left[E+\frac{v^2}{2}+\frac{x^2-(x-X)^2}{2}\right]f
=\left[E+Xx+\frac{v^2-X^2}{2}\right]f.
$$

It is satisfied provided

$$
\ddot X=-X,\qquad \dot\gamma=\frac{X^2-\dot X^2}{2}.
$$

Since $d(X\dot X)/dt=\dot X^2-X^2$ for this oscillator, an explicit phase and trajectory are

$$
\boxed{X(t)=a\cos t+b\sin t,\qquad
\Theta(x,t)=\dot X(t)\left(x-\frac{X(t)}2\right)-Et+\Theta_0.}
$$

Thus [harmonic-trap translation of a nonlinear Schrödinger soliton](../../../../../harmonic-trap-translation-of-a-nonlinear-schrodinger-soliton.md) is exact: the trapped profile translates without changing its shape, even though its centre accelerates.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
