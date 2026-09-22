<h1 id="33e/solution">Solution</h1>

↑ **Parent:** [33E](../33e.md)

Equality of the mixed derivatives of the auxiliary vector $\Psi$ gives

$$
\Psi_{xt}=U_t\Psi+UV\Psi,
\qquad
\Psi_{tx}=V_x\Psi+VU\Psi.
$$

Thus the [zero-curvature condition](../../../../../zero-curvature-condition.md) for this convention is

$$
\boxed{U_t-V_x+[U,V]=0}.
$$

Substituting the displayed matrices and collecting powers of the spectral parameter $\lambda$ makes every diagonal entry and every $\lambda$-dependent term cancel. The remaining matrix is

$$
U_t-V_x+[U,V]
=
\begin{pmatrix}
0&iq_t-q_{xx}-2rq^2\\
 ir_t+r_{xx}+2qr^2&0
\end{pmatrix}.
$$

Consequently compatibility is equivalent to

$$
\boxed{
 ir_t+r_{xx}+2qr^2=0,
\qquad
 iq_t-q_{xx}-2rq^2=0
},
$$

so the requested constant is

$$
\boxed{a=2}.
$$

This is the [AKNS Lax pair for the nonlinear Schrodinger equation](../../../../../akns-lax-pair-for-the-nonlinear-schrodinger-equation.md).

The reduction

$$
q=\overline r
$$

is preserved by the two equations, which become complex conjugates and reduce to the [Focusing nonlinear Schrodinger equation](../../../../../focusing-nonlinear-schrodinger-equation.md)

$$
\boxed{ir_t+r_{xx}+2|r|^2r=0}.
$$

The analogous reduction

$$
q=-\overline r
$$

gives the [Defocusing nonlinear Schrödinger equation](../../../../../defocusing-nonlinear-schrodinger-equation.md)

$$
\boxed{ir_t+r_{xx}-2|r|^2r=0}.
$$

For a complex field $r$ and rapidly decreasing boundary conditions, define

$$
H_{\mathrm{foc}}[r,\overline r]
=\int_{\mathbb R}\left(|r_x|^2-|r|^4\right)dx,
\qquad
H_{\mathrm{def}}[r,\overline r]
=\int_{\mathbb R}\left(|r_x|^2+|r|^4\right)dx.
$$

Their [variational derivatives](../../../../../variational-derivative.md), after [integration by parts](../../../../../integration-by-parts.md), are

$$
\frac{\delta H_{\rm foc}}{\delta\overline r}
=-r_{xx}-2|r|^2r,
\qquad
\frac{\delta H_{\rm def}}{\delta\overline r}
=-r_{xx}+2|r|^2r.
$$

Both equations therefore have the [Hamiltonian field equation](../../../../../hamiltonian-field-equation.md)

$$
\boxed{
ir_t=\frac{\delta H}{\delta\overline r}
},
$$

or, including the conjugate equation,

$$
\begin{pmatrix}r_t\\ \overline r_t\end{pmatrix}
=
\begin{pmatrix}0&-i\\ i&0\end{pmatrix}
\begin{pmatrix}\delta H/\delta r\\ \delta H/\delta\overline r\end{pmatrix}.
$$

This is the [Hamiltonian form of the cubic nonlinear Schrodinger equations](../../../../../hamiltonian-form-of-the-cubic-nonlinear-schrodinger-equations.md).

Now put

$$
r(x,t)=e^{-iEt}f(x),
$$

where $E$ and $f$ are real and $f$ is smooth and rapidly decreasing. For the focusing equation,

$$
f''+Ef+2f^3=0.
$$

Multiplication by $f'$ and use of the decay at infinity gives the first integral

$$
(f')^2=-Ef^2-f^4.
$$

A nonzero solution requires $E<0$. Writing $E=-\kappa^2$ with $\kappa>0$, separation of variables, or direct substitution, gives

$$
\boxed{
f(x)=\pm\kappa\operatorname{sech}\bigl(\kappa(x-x_0)\bigr)
}.
$$

Hence

$$
\boxed{
r(x,t)=\pm\kappa e^{i\kappa^2t}
\operatorname{sech}\bigl(\kappa(x-x_0)\bigr)
}
$$

is the [Bright standing soliton of the focusing nonlinear Schrodinger equation](../../../../../bright-standing-soliton-of-the-focusing-nonlinear-schrodinger-equation.md).

For the defocusing equation the profile instead satisfies

$$
f''+Ef-2f^3=0,
$$

with first integral

$$
(f')^2=f^4-Ef^2=f^2(f^2-E).
$$

If a nonzero rapidly decreasing profile existed, $|f|$ would attain a positive maximum $A$. At that point $f'=0$, so the identity forces $E=A^2>0$. But along either tail, where $0<|f|<A$, the right-hand side $f^2(f^2-E)$ is negative, which is impossible. Thus there is no nonzero solution of the prescribed form, as recorded by [No rapidly decaying standing wave for the defocusing cubic nonlinear Schrodinger equation](../../../../../no-rapidly-decaying-standing-wave-for-the-defocusing-cubic-nonlinear-schrodinger-equation.md).

## ↑ Ancestors (10)

1. [33E](../33e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
