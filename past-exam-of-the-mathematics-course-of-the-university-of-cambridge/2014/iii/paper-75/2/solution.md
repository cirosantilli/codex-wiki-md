<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Suppress the common time factor $e^{i\omega t}$, take $\omega>0$, and fix the spatial [Fourier transform](../../../../../fourier-transform.md) convention

$$
\Phi(k,y)=\int_{-\infty}^{\infty}\phi(x,y)e^{ikx}\,dx,\qquad
\phi(x,y)=\frac1{2\pi}\int_\Gamma\Phi(k,y)e^{-ikx}\,dk.
$$

A plus transform is supported on $x>0$ and analytic above $\Gamma$; a minus transform is supported on $x<0$ and analytic below it. For the outgoing [radiation condition](../../../../../radiation-condition.md) with this time convention, initially take $k_0=\omega/c_0-i\varepsilon$, $\varepsilon>0$, and pass to the limit at the end. Thus $+k_0$ lies below the contour and $-k_0$ above it.

Choose $\gamma=(k^2-k_0^2)^{1/2}$ to have positive real part on the real transform line. Its [branch cuts](../../../../../branch-cut.md) run from $+k_0$ into the lower half-plane and from $-k_0$ into the upper half-plane, without crossing $\Gamma$; downward and upward vertical rays are suitable. In the zero-absorption limit, $\gamma>0$ for real $|k|>k_0$ and $\gamma=+i\sqrt{k_0^2-k^2}$ between the branch points. This ensures that $e^{-\gamma|y|}$ represents decay or outgoing radiation, rather than an incoming exterior field.

Evenness in $y$ and the [Helmholtz equation](../../../../../helmholtz-equation.md) give the transformed fields

$$
\Phi=A(k)\cosh(\gamma y)\quad(|y|<b),\qquad
\Phi=B(k)e^{-\gamma(|y|-b)}\quad(|y|>b).
$$

At $y=b$, the one-sided normal derivatives of the scattered field agree for $x<0$, because that part of the interface is open. For $x>0$ they both vanish by rigidity. Their common trace is therefore a minus function, denoted $V^-(k)=\partial_y\Phi^-|_{y=b}$. Consequently

$$
A=\frac{V^-}{\gamma\sinh(\gamma b)},\qquad B=-\frac{V^-}{\gamma}.
$$

The jump in the total scattered transform is

$$
J=\Phi(b^+)-\Phi(b^-)
=-\frac{V^-}{\gamma}\{1+\coth(\gamma b)\}
=-\frac{V^-}{L},\qquad L=\gamma\sinh(\gamma b)e^{-\gamma b}.
$$

For $x<0$, continuity of the total [mass density](../../../../../density.md) requires the scattered jump to cancel the incident jump, so $\phi(b^+)-\phi(b^-)=e^{ik_0x}$. Its minus transform is $-i/(k+k_0)$. The unknown plate-side jump is the plus function $J^+=[\Phi^+]_{b^-}^{b^+}$. Thus $J=J^+-i/(k+k_0)$, and the [Wiener-Hopf equation](../../../../../wiener-hopf-equation.md) follows:

$$
\boxed{\frac{V^-}{L}+J^+=\frac{i}{k+k_0}.}
$$

Use the [Wiener-Hopf factorization](../../../../../wiener-hopf-factorization.md) $L=L^+L^-$, with factors analytic and nonzero in their designated half-planes. Their analytic continuations allocate outgoing modal zeros to $L^+$ below the contour, and the opposite zeros to $L^-$ above it. Set $C=L^+(-k_0)$. Multiplication by $L^+$ and pole subtraction give

$$
\frac{V^-}{L^-}-\frac{iC}{k+k_0}
=-L^+J^++\frac{i(L^+(k)-C)}{k+k_0}=E(k).
$$

The pole in the upper expression is removable by its numerator. The two expressions analytically continue to the common entire function, which is zero under the stipulated edge/growth assumption. Hence

$$
V^-=\frac{iCL^-}{k+k_0},\qquad
J^+=\frac{i}{k+k_0}\left(1-\frac{C}{L^+}\right),
$$

and the transformed fields are

$$
\boxed{\Phi(k,y)=\frac{iCL^-(k)\cosh(\gamma y)}{(k+k_0)\gamma\sinh(\gamma b)}\quad(|y|<b),}
$$



$$
\boxed{\Phi(k,y)=-\frac{iCL^-(k)}{(k+k_0)\gamma}e^{-\gamma(|y|-b)}
=-\frac{iC\sinh(\gamma b)}{(k+k_0)L^+(k)}e^{-\gamma|y|}\quad(|y|>b).}
$$

A constant reciprocal rescaling of the factors does not alter $CL^-$ or the physical field.

Inside the guide, $\cosh(\gamma y)$ and $\gamma\sinh(\gamma b)$ are even entire functions of $\gamma$, while $L^-$ is analytic in the lower half-plane. Thus continuation across the lower [branch cut](../../../../../branch-cut.md) changes none of the interior transform: that cut is removable. The exterior expression retains the cut, corresponding to radiation into the open exterior.

For $x>0$, the inverse-transform contour closes downwards, clockwise. Away from modal cutoffs, its enclosed singularities are the outgoing simple poles

$$
k_n=\sqrt{k_0^2-(n\pi/b)^2},\qquad n=0,1,\ldots,
$$

with positive real part for propagating modes and negative imaginary part for decaying modes; $k_0$ is the $n=0$ root. The opposite roots lie above the contour or cancel against zeros of $L^-$. Symmetry excludes odd transverse modes. At $n\geq1$, $\gamma=i n\pi/b$, and differentiation of $D(k)=\gamma\sinh(\gamma b)$ gives

$$
D'(k_n)=b k_n(-1)^n,\qquad D'(k_0)=2bk_0.
$$

Each inverse-transform contribution is $-i$ times its [residue](../../../../../residue.md). Therefore the [outgoing modes of an open rigid acoustic waveguide](../../../../../outgoing-modes-of-an-open-rigid-acoustic-waveguide.md) are

$$
\boxed{\phi(x,y)=A_0e^{-ik_0x}
+\sum_{n=1}^{\infty}A_n\cos\left(\frac{n\pi y}{b}\right)e^{-ik_nx},}
$$



$$
\boxed{A_0=\frac{L^+(-k_0)L^-(k_0)}{4bk_0^2},\qquad
A_n=\frac{(-1)^nL^+(-k_0)L^-(k_n)}{bk_n(k_n+k_0)}\quad(n\geq1).}
$$

The original time factor multiplies this expression. Thus every cut-on mode propagates in the positive $x$ direction; cut-off modes are [evanescent waves](../../../../../evanescent-wave.md) decaying into the guide, not additional backward waves. Strictly, a complete mode sum includes these evanescent modes as well as propagating ones. The displayed simple-pole amplitudes apply away from exact cutoffs; cutoff values use the outgoing limiting-absorption continuation before taking the limit. **The reflected plane-wave amplitude relative to the unit incident wave is $A_0$ above.** It has the expected negative sign in the long-wavelength leading kernel approximation $L\simeq b(k^2-k_0^2)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
