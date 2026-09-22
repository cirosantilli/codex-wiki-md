<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Linearity permits subtraction of the incident [acoustic membrane wave](../../../../../../acoustic-wave-on-a-tensioned-massive-membrane.md). The scattered [pressure](../../../../../../pressure.md) solves the homogeneous [Helmholtz equation](../../../../../../helmholtz-equation.md), and the kinematic relation defines its line displacement $\eta'$ on both halves. On $x<0$, subtracting the incident [elastic membrane](../../../../../../elastic-membrane.md) equation gives the scattered dynamic equation. On $x>0$, there is no [elastic membrane](../../../../../../elastic-membrane.md), so the total [pressure](../../../../../../pressure.md) jump must vanish, giving $[p']=-[p_I]$. The pinned endpoint has $\eta(0)=0$, hence **$\eta'(0)=-1$**, rather than zero.

Use full and [Half-range Fourier transforms](../../../../../../half-range-fourier-transform.md) with the same $e^{ikx}$ convention as part (a), and put

$$
\beta=\rho_0\omega^2,\quad a(k)=m\omega^2-Tk^2,\quad A=\eta_x(0),\quad\kappa=k-k_I.
$$

Write $P^-$ for the left transform of the upper scattered [pressure](../../../../../../pressure.md), $P^+$ for its right transform, and $\eta^\pm$ for the corresponding transforms of $\eta'$. Outgoing antisymmetry in $y$ implies

$$
\eta^-+\eta^+=-\frac\gamma\beta(P^-+P^+),\qquad P^+=\frac{i\beta}{\kappa\gamma_I}.
$$

The second relation comes from the prescribed [pressure](../../../../../../pressure.md) cancellation on $x>0$.

The endpoint terms in the left [Fourier transform](../../../../../../fourier-transform.md) of $\eta'_{xx}$ are crucial:

$$
\int_{-\infty}^0e^{ikx}\eta'_{xx}dx=\eta'_x(0)-ik\eta'(0)-k^2\eta^-=A+i(k+k_I)-k^2\eta^-.
$$

Thus $2P^-=a\eta^-+TA+iT(k+k_I)$. Eliminating $\eta^-$ gives the [Wiener-Hopf equation](../../../../../../wiener-hopf-equation.md)

$$
\boxed{K(k)P^-(k)+\eta^+(k)=\frac{TA}{a(k)}+\frac{iT(k+k_I)}{a(k)}-\frac{i\gamma(k)}{(k-k_I)\gamma_I},\qquad K(k)=\frac2{a(k)}+\frac{\gamma(k)}\beta.}
$$

There is a defect in the printed right side: with the stated incident exponential, [pressure](../../../../../../pressure.md) jump, and pinned total displacement, it omits the incident endpoint term and has the opposite sign on the incident-pressure term. The displayed corrected equation follows directly from both boundary traces. The given right side cannot be derived with these definitions. Using $a(k_I)=-2\beta/\gamma_I$, an especially useful equivalent form is

$$
K P^-+\eta^+=\frac{TA}{a}-\frac i\kappa-\frac{i\beta K}{\kappa\gamma_I}.
$$

The correction is necessary for the reconstructed [pressure](../../../../../../pressure.md) to satisfy the original physical boundary conditions.

For [Wiener-Hopf factorization](../../../../../../wiener-hopf-factorization.md), take $K=K^+K^-$ with the plus factor analytic and nonzero in the upper half-plane and the minus factor analytic and nonzero in the lower half-plane. Singularities listed next refer to continuation out of each factor's own analytic half-plane. Let $b=\omega\sqrt{m/T}$, so $a=-T(k-b)(k+b)$ and $b$ lies below the real axis. Generically $K^+$ inherits the [pole](../../../../../../pole.md) at $b$ and the square-root [branch point](../../../../../../branch-point.md) at $k_0$, while $K^-$ inherits the [pole](../../../../../../pole.md) at $-b$ and the [branch point](../../../../../../branch-point.md) at $-k_0$. The kernel is finite but nonanalytic at the acoustic branch points: its local behavior is a constant plus a square-root term, not an inverse-square-root divergence. Coincident branch points and poles require a limiting treatment.

Zeros of $K$ are the fluid-loaded [dispersion relation](../../../../../../dispersion-relation.md) roots. Lower-half-plane roots, including the incoming guided root $k_I$, belong to the continued $K^+$; upper-half-plane roots, including the reflected root $-k_I$ for the even kernel, belong to the continued $K^-$. The roots represent membrane-guided modes; the branch cuts represent radiated acoustic waves. Only roots on the selected outgoing sheet are included, not spurious roots created by squaring the dispersion relation. No explicit factorization is required.

Here is an explicit solution in terms of those factors. Define

$$
B(k)=\frac{T}{a(k)K^+(k)},\qquad C=\frac{1}{2bK^+(-b)},\qquad B^-(k)=\frac C{k+b},\qquad B^+(k)=B(k)-\frac C{k+b}.
$$

The [pole](../../../../../../pole.md) of $B$ at $-b$ has residue $C$; the [pole](../../../../../../pole.md) at $b$ is canceled by the [pole](../../../../../../pole.md) of $K^+$. Thus $B^\pm$ have the required respective analyticity. Divide the corrected [Wiener-Hopf equation](../../../../../../wiener-hopf-equation.md) by $K^+$ and split its right side as $F^++F^-$, where

$$
\begin{aligned}
F^-&=A\frac C{k+b}-\frac{i\beta}{\gamma_I}\frac{K^-(k)-K^-(k_I)}{k-k_I},\\
F^+&=AB^+(k)-\frac{i}{(k-k_I)K^+(k)}-\frac{i\beta K^-(k_I)}{(k-k_I)\gamma_I}.
\end{aligned}
$$

The difference quotient in $F^-$ is removable at $k_I$ and is analytic below. Moving the plus and minus terms to opposite sides yields the common [entire function](../../../../../../entire-function.md). With the assumed **$E(k)=0$**, the solution is

$$
\boxed{P^-=\frac{F^-}{K^-},\qquad\eta^+=K^+F^+.}
$$

Combining $P^-$ with the known $P^+$ gives the full scattered [pressure](../../../../../../pressure.md) transform

$$
P^-+P^+=\frac1{K^-(k)}\left[\frac{AC}{k+b}+\frac{i\beta K^-(k_I)}{(k-k_I)\gamma_I}\right].
$$

The requested [pressure](../../../../../../pressure.md) integral, for $y\ne0$, is consequently

$$
\boxed{p(x,y)=p_I(x,y)+\frac{\operatorname{sgn}(y)}{2\pi}\int_{\mathcal C}e^{-ikx-\gamma(k)|y|}\frac1{K^-(k)}\left[\frac{AC}{k+b}+\frac{i\beta K^-(k_I)}{(k-k_I)\gamma_I}\right]dk.}
$$

The real contour $\mathcal C$ uses the causal continuation $\operatorname{Im}\omega<0$; its undamped limit retains the induced [pole](../../../../../../pole.md) and branch-cut prescriptions. The [residue theorem](../../../../../../residue-theorem.md) shows that upper-half-plane zeros of $K^-$ yield left-going scattered [elastic membrane](../../../../../../elastic-membrane.md) modes. On the right, the lower incident-pole residue of the scattered integral cancels $p_I$ at the open line, as required.

Finally reconstruct the left scattered displacement:

$$
\boxed{\eta^-=\frac{2P^- -TA-iT(k+k_I)}{a(k)}.}
$$

For a generic unspecified $A$, this has a lower-half-plane [pole](../../../../../../pole.md) at the bare [elastic membrane](../../../../../../elastic-membrane.md) wavenumber $b$. Such a [pole](../../../../../../pole.md) is incompatible with analyticity of an outgoing left-supported scattered displacement: it would represent an additional right-going incoming [elastic membrane](../../../../../../elastic-membrane.md) contribution. It must be removed. Its residue is $-[2P^-(b)-TA-iT(b+k_I)]/(2Tb)$, so the [incoming-pole cancellation at a pinned membrane edge](../../../../../../incoming-pole-cancellation-at-a-pinned-membrane-edge.md) condition is

$$
\boxed{2P^-(b)-TA-iT(b+k_I)=0.}
$$

Since $P^-$ is linear in $A$, this fixes the endpoint slope generically. Explicitly it is

$$
A\left[T-\frac{C}{bK^-(b)}\right]=\frac{2i\beta K^-(k_I)}{(b-k_I)\gamma_I K^-(b)}.
$$

The physical lower incident [pole](../../../../../../pole.md) of the total displacement is already prescribed by $\eta_I$; it must not be confused with this removable spurious [pole](../../../../../../pole.md) of the scattered field.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
