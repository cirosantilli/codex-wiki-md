<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Suppress the common time factor $e^{i\omega t}$ and use the [Fourier transform](../../../../../fourier-transform.md) convention

$$
\widetilde\phi(k,y)=\int_{\mathbb R}e^{ikx}\phi(x,y)\,dx,\qquad \phi(x,y)=\frac{1}{2\pi}\int_\Gamma e^{-ikx}\widetilde\phi(k,y)\,dk.
$$

A right [Half-range Fourier transform](../../../../../half-range-fourier-transform.md) is analytic above its convergence line and a left transform below it. For the [limiting absorption principle](../../../../../limiting-absorption-principle.md) with this time convention take $\omega=\omega_r-i\varepsilon$, $\omega_r>0$, $\varepsilon>0$, before taking $\varepsilon\downarrow0$. Set

$$
\gamma(k)=\sqrt{k^2-\omega^2},\qquad \operatorname{Re}\gamma(k)>0\quad(k\in\mathbb R).
$$

This is the [outgoing acoustic square-root branch](../../../../../outgoing-acoustic-square-root-branch.md): at a propagating real wavenumber, $\gamma\to i\sqrt{\omega_r^2-k^2}$. Put $J=[\widetilde\phi]_{y=-0}^{y=+0}$ and $d^+=\partial_y\Phi^+(k,0)$. Across the fluid part of $y=0$, the field and its normal derivative are continuous; on the sheet both sides have the same normal velocity. The outgoing [Helmholtz equation](../../../../../helmholtz-equation.md) solutions therefore have equal normal derivatives and opposite scattered traces:

$$
\widetilde\phi(k,y)=\begin{cases}\frac12J(k)e^{-\gamma y},&y>0,\\-\frac12J(k)e^{\gamma y},&y<0,\end{cases}\qquad \widetilde\phi_y(k,0)=-\frac{\gamma J}{2}.
$$

The jump $J$ is supported on $x<0$, and so is a minus transform.

The linear fluid equation $i\omega v_y=-\partial_y\rho'$ and the sheet velocity $v_y=i\omega\eta$ imply $\partial_y\rho'=\omega^2\eta$ on either face. The incident contribution to the left derivative transform is $\omega\sin\theta_0/(k+\omega\cos\theta_0)$. Writing $\eta^- =\int_{-\infty}^0e^{ikx}\eta(x)\,dx$, it follows that

$$
-\frac{\gamma J}{2}=\omega^2\eta^- -\frac{\omega\sin\theta_0}{k+\omega\cos\theta_0}+d^+.
$$

The upward net pressure is lower minus upper, hence $P=-J$ in transform space. If $s=\eta'(0)$, the pinned endpoint gives

$$
\widetilde{\eta''}^{\,-}=s-k^2\eta^-,\qquad J=(m\omega^2-Tk^2)\eta^-+Ts.
$$

Combining these identities gives the [Wiener-Hopf equation](../../../../../wiener-hopf-equation.md)

$$
\boxed{K(k)J(k)+d^+(k)=F(k),\qquad K(k)=\frac{\gamma(k)}2+\frac{\omega^2}{m\omega^2-Tk^2},}
$$



$$
F(k)=\frac{\omega\sin\theta_0}{k+\omega\cos\theta_0}+\frac{T\omega^2s}{m\omega^2-Tk^2}.
$$

This is the [plane-wave forcing of a pinned elastic half-sheet](../../../../../plane-wave-forcing-of-a-pinned-elastic-half-sheet.md).

Let $b=\omega\sqrt{m/T}$ and assume initially that the distinguished points are distinct. Besides the branch points $\pm\omega$, $K$ has simple poles at $\pm b$. Its physical-sheet zeros $\pm k_s$ solve the fluid-loaded [dispersion relation](../../../../../dispersion-relation.md)

$$
\gamma(k_s)(Tk_s^2-m\omega^2)=2\omega^2.
$$

For real positive frequency there is exactly one positive real root $k_s>\max(\omega_r,\omega_r\sqrt{m/T})$: the left side increases strictly from zero to infinity on that interval. Equivalently, with $q=\gamma(k_s)>0$, $Tq^3+(T-m)\omega_r^2q-2\omega_r^2=0$. Its other roots have negative real part and do not belong to this outgoing sheet. Continue $k_s$ with small absorption; $+\omega,+b,+k_s$ lie below the real line and their negative partners above it. The [Wiener-Hopf factorization](../../../../../wiener-hopf-factorization.md) assigns the lower branch cut and pole to $K^+$, and the upper branch cut and pole to $K^-$. The continued $K^+$ has a zero at $+k_s$, and $K^-$ at $-k_s$; these are poles of their reciprocals, rather than poles of the factors. Branch cuts can be drawn away from the real line into the corresponding half-planes.

For this standard assignment a common strip of analyticity and nonvanishing is

$$
\boxed{\mathcal D=\{k:-d<\operatorname{Im}k<d\},\qquad d=\min\{\varepsilon,\ \varepsilon\sqrt{m/T},\ -\operatorname{Im}k_s\}>0.}
$$

The strip shrinks to the real contour as absorption is removed. The factors continue meromorphically beyond their designated half-planes; the allocation of the poles and branch points is part of the [radiation condition](../../../../../radiation-condition.md). The incident pole $-\omega\cos\theta_0$ belongs above the inversion contour. For incidence with $0<\theta_0<\pi/2$ the real contour is a direct choice. Other nongrazing angles are obtained by [analytic continuation](../../../../../analytic-continuation.md) with the incident pole kept on its prescribed side, deforming the contour locally if necessary. Coincident distinguished points and grazing incidence are treated by the corresponding limits, not by dividing by a coincident pole.

Divide the [Wiener-Hopf equation](../../../../../wiener-hopf-equation.md) by $K^+$ and use [pole subtraction in a Wiener-Hopf equation](../../../../../pole-subtraction-in-a-wiener-hopf-equation.md). With $a=\omega\cos\theta_0$, the minus part of $F/K^+$ is

$$
B^-(k)=\frac{\omega\sin\theta_0}{K^+(-a)(k+a)}+\frac{\omega^2s}{2bK^+(-b)(k+b)}.
$$

Indeed these are exactly the incident-pole and upper bare-sheet-pole residues. At the lower bare-sheet pole $+b$, the forcing pole is canceled by the pole of $K^+$ before splitting. Thus $B^+=F/K^+-B^-$ is analytic on the plus side of the contour. The separated equation is

$$
K^-J-B^-=B^+-d^+/K^+=E.
$$

With the stipulated $E=0$,

$$
J=\frac{B^-}{K^-},\qquad d^+=K^+B^+=F-K^+B^-.
$$

The scattered field is consequently

$$
\boxed{\phi(x,y)=\frac{\operatorname{sgn}y}{4\pi}\int_\Gamma e^{-ikx-\gamma(k)|y|}\frac{B^-(k)}{K^-(k)}\,dk,\qquad y\ne0.}
$$

The full time-dependent density perturbation is the incident field plus $e^{i\omega t}\phi$. The two traces at $y=0$ follow by limiting from above and below. A constant rescaling of the two factors does not change this field.

To determine the endpoint slope, reconstruct the sheet transform using the fluid condition:

$$
\eta^-(k)=\frac1{\omega^2}\left[-\frac{\gamma J}{2}-d^++\frac{\omega\sin\theta_0}{k+a}\right]=\frac{J-Ts}{m\omega^2-Tk^2}.
$$

At $+b$ the continued $K^+$ has residue $-\omega^2/(2TbK^-(b))$. Therefore the derivative transform $d^+$ generically has the lower-plane pole

$$
\operatorname{Res}_{k=b}d^+=-\frac{\omega^2s}{2b}+\frac{\omega^2B^-(b)}{2TbK^-(b)}.
$$

This pole produces a forbidden incoming bare-sheet wave in the reconstructed displacement: $e^{i\omega t-ibx}$ travels towards the endpoint from $x=-\infty$. A minus transform of the specified outgoing solution must be analytic there. The [incoming-pole cancellation at a pinned membrane edge](../../../../../incoming-pole-cancellation-at-a-pinned-membrane-edge.md) is precisely

$$
\boxed{B^-(b)=TsK^-(b),\qquad J(b)=Ts.}
$$

For generic parameters this determines

$$
\boxed{s=\frac{\omega\sin\theta_0}{K^+(-a)(b+a)\left[TK^-(b)-\dfrac{\omega^2}{4b^2K^+(-b)}\right]}.}
$$

The lower pole is removed; the upper zero $-k_s$ of $K^-$ can still produce the legitimate outgoing [evanescent acoustic surface wave](../../../../../evanescent-acoustic-surface-wave.md), whose phase travels to negative $x$. This distinction separates the spurious bare-sheet wave from the coupled fluid-loaded mode. No explicit factorization has been used.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
