<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a stationary finite-[wavenumber](../../../../../wavenumber.md) instability, the relevant Landau–Ginzburg model is the [real Ginzburg–Landau equation](../../../../../real-ginzburg-landau-equation.md): its coefficients are real although its pattern amplitude is complex. The [complex amplitude](../../../../../complex-amplitude.md) records both the strength and the position of the underlying pattern. Assume a simple critical pair of [Fourier modes](../../../../../fourier-mode.md) $\pm k_c$, a quadratic nondegenerate maximum of the linear [growth rate](../../../../../growth-rate.md), and no additional conserved or marginal mode. The last assumption is essential: the conserved field in the previous problem requires an additional evolution equation.

To derive the model, write a real evolution equation schematically as $u_t=L(r)u+N_2(u,u)+N_3(u,u,u)+\cdots$, with symmetric multilinear nonlinearities. Put $r=\varepsilon^2r_2$, $X=\varepsilon x$, $T=\varepsilon^2t$ and use the [method of multiple scales](../../../../../method-of-multiple-scales.md) expansion

$$
u=\varepsilon\left[A(X,T)v e^{ik_cx}+\overline A(X,T)\overline v e^{-ik_cx}\right]+\varepsilon^2u_2+\varepsilon^3u_3+\cdots.
$$

Here $L(k_c;0)v=0$. At the next order the noncritical mean and second harmonic are slaved to the critical mode:

$$
u_2=|A|^2w_0+A^2w_2e^{2ik_cx}+\overline A^{\,2}\overline w_2e^{-2ik_cx}+\text{gradient corrections},
$$

where $L(0;0)w_0=-2N_2(v,\overline v)$ and $L(2k_c;0)w_2=-N_2(v,v)$. These inverses exist under the no-other-critical-mode hypothesis. Let $v^*$ be an adjoint null vector normalized by $\langle v^*,v\rangle=1$. At order $\varepsilon^3$, the [Fredholm solvability condition](../../../../../fredholm-solvability-condition.md) requires the resonant forcing to be orthogonal to $v^*$. The cubic resonant contribution is

$$
\kappa=\left\langle v^*,\,3N_3(v,v,\overline v)+2N_2(v,w_0)+2N_2(\overline v,w_2)\right\rangle.
$$

This shows why the cubic coefficient includes feedback from slaved harmonics as well as any original cubic nonlinearity. The resulting [amplitude equation](../../../../../amplitude-equation.md), after naming its linear control coefficient $\mu$, is

$$
\boxed{A_T=\mu A+\xi A_{XX}-g|A|^2A,\qquad \xi=-\tfrac12\lambda''(k_c)>0,\quad g=-\kappa.}
$$

Here $\lambda(k)$ is the critical linear [dispersion relation](../../../../../dispersion-relation.md) for growth. The condition $g>0$ gives a [supercritical bifurcation](../../../../../supercritical-bifurcation.md); $g<0$ calls for higher-order saturation, for example the [quintic real Ginzburg-Landau equation](../../../../../quintic-real-ginzburg-landau-equation.md).

A concrete check is the cubic [Swift–Hohenberg equation](../../../../../swift-hohenberg-equation.md) $u_t=\varepsilon^2\mu u-(1+\partial_x^2)^2u-g_0u^3$. With $u=\varepsilon(Ae^{ix}+\overline A e^{-ix})+\cdots$, its linear operator contributes $4A_{XX}$ at resonant order, while the cubic resonance is $3|A|^2A$. Hence $A_T=\mu A+4A_{XX}-3g_0|A|^2A$. This directly realizes the perturbation-theory coefficients above.

Symmetry independently constrains the form. A fast spatial [translation](../../../../../translation-geometry.md) rotates $A$ by a constant phase, so every nondifferential monomial must transform like $A$. The leading allowed nonlinear term is $|A|^2A$, and a quadratic term is forbidden. A spatial [reflection](../../../../../reflection-mathematics.md) maps $A(X)$ to $\overline A(-X)$; it makes the leading coefficients real and rules out a drift term in a reflection-symmetric rest frame. The vanishing first [derivative](../../../../../derivative.md) of the linear [growth rate](../../../../../growth-rate.md) at $k_c$ is consistent with the absence of a leading first spatial [derivative](../../../../../derivative.md). These arguments constrain terms but do not calculate $\xi,g$ or replace the solvability calculation. Breaking [reflection](../../../../../reflection-mathematics.md) or studying an oscillatory instability generally leads to the [complex Ginzburg–Landau equation](../../../../../complex-ginzburg-landau-equation.md) with genuinely complex coefficients.

The principal steady solutions are the zero state and the [Ginzburg-Landau plane waves](../../../../../ginzburg-landau-plane-wave.md)

$$
\boxed{A=R e^{i(qX+\theta_0)},\qquad R^2=\frac{\mu-\xi q^2}{g}>0.}
$$

Their physical carrier [wavenumber](../../../../../wavenumber.md) is $k_c+\varepsilon q$. For $q=0$ the constant phase is arbitrary, giving a circle of uniform-amplitude states. The zero state has Fourier [growth rate](../../../../../growth-rate.md) $\mu-\xi p^2$ and is stable for $\mu<0$. For $g>0$, each existing plane wave is stable to spatially homogeneous amplitude perturbations, with radial [eigenvalue](../../../../../eigenvalue.md) $-2gR^2$, and neutral to a constant phase shift.

Steady modulated states are also possible. Writing $A=a(X)e^{i\phi(X)}$ gives the conserved spatial phase current $j=a^2\phi_X$ and

$$
\xi a_{XX}+\mu a-ga^3-\frac{\xi j^2}{a^3}=0.
$$

Its [first integral](../../../../../first-integral.md) is $\xi a_X^2/2+\mu a^2/2-ga^4/4+\xi j^2/(2a^2)=E$. [Boundary conditions](../../../../../boundary-condition.md) select nonuniform periodic amplitudes, [fronts](../../../../../front-solution.md) or defects from this spatial dynamics. In the invariant real subspace, for example,

$$
A=\sqrt{\mu/g}\,\tanh\left(\sqrt{\mu/(2\xi)}X\right)
$$

is a steady kink joining opposite real states. It is not stable in the unrestricted complex equation: the imaginary perturbation $v=\operatorname{sech}(\sqrt{\mu/(2\xi)}X)$ has [eigenvalue](../../../../../eigenvalue.md) $\mu/2>0$ under $v_T=\xi v_{XX}+(\mu-gA^2)v$. This illustrates why a real-amplitude calculation can miss a phase instability. With real coefficients the [Lyapunov functional](../../../../../lyapunov-functional.md)

$$
\mathcal F[A]=\int\left(\xi|A_X|^2-\mu|A|^2+\frac g2|A|^4\right)dX
$$

satisfies $A_T=-\delta\mathcal F/\delta\overline A$ and $d\mathcal F/dT=-2\int|A_T|^2dX$ under compatible [boundary conditions](../../../../../boundary-condition.md). It supplies a variational structure absent from a generic complex-coefficient model.

To test full [linear stability](../../../../../linear-stability.md) of a plane wave, set $A=e^{iqX}(R+u+iv)$ with real perturbations $u,v$. Let $b=gR^2=\mu-\xi q^2>0$. The linear equations are

$$
u_T=\xi u_{XX}-2\xi qv_X-2bu,\qquad v_T=\xi v_{XX}+2\xi qu_X.
$$

For perturbation [wavenumber](../../../../../wavenumber.md) $p$, the [sideband spectrum of a real Ginzburg-Landau plane wave](../../../../../sideband-spectrum-of-a-real-ginzburg-landau-plane-wave.md) is

$$
\boxed{\sigma_\pm=-\xi p^2-b\pm\sqrt{b^2+4\xi^2q^2p^2}.}
$$

The phase branch at small $p$ is

$$
\sigma_+=-\xi\frac{\mu-3\xi q^2}{\mu-\xi q^2}p^2+O(p^4).
$$

Therefore the robust stable band on the infinite line is $q^2<\mu/(3\xi)$, narrower than the existence band $q^2<\mu/\xi$. Crossing its boundary gives the longitudinal [Eckhaus instability](../../../../../eckhaus-instability.md). At the boundary the quadratic phase-diffusion coefficient vanishes and the leading nonzero term is negative of order $p^4$. More exactly, a nonzero [sideband](../../../../../spatial-sideband.md) grows only when $p^2<6q^2-2\mu/\xi$; a finite periodic domain for the [wave envelope](../../../../../envelope-waves.md) may exclude that interval. Constant-amplitude stability is understood modulo its neutral global phase, and the allowed perturbation [wavenumbers](../../../../../wavenumber.md) must always be specified.

In a second spatial dimension, an anisotropic medium that selects one roll orientation permits an equation with $\xi_xA_{XX}+\xi_yA_{YY}$. For positive coefficients its plane-wave analysis is similar, with the second-dimensional contribution adding damping. But simply replacing $A_{XX}$ by an isotropic Laplacian is not a faithful extension for rotationally invariant stationary rolls. There the critical wavevectors form a circle. Near $(k_c,0)$,

$$
\left|(k_c+\varepsilon q,\varepsilon^{1/2}p)\right|=k_c+\varepsilon\left(q+\frac{p^2}{2k_c}\right)+O(\varepsilon^2).
$$

This forces the [anisotropic transverse scaling of an isotropic roll envelope](../../../../../anisotropic-transverse-scaling-of-an-isotropic-roll-envelope.md): $X=\varepsilon x$, $Y=\varepsilon^{1/2}y$, $T=\varepsilon^2t$. For the positive carrier convention used here the [Newell–Whitehead–Segel equation](../../../../../newell-whitehead-segel-equation.md) is

$$
\boxed{A_T=\mu A+\xi\left(\partial_X-\frac{i}{2k_c}\partial_Y^2\right)^2A-g|A|^2A.}
$$

The opposite fast-carrier convention reverses the accompanying imaginary sign and detuning convention. For a transverse phase perturbation of $A=Re^{iqX}$ our convention gives $\sigma=-\xi qp^2/k_c-\xi p^4/(4k_c^2)$. Thus $q<0$ permits the transverse [zigzag instability](../../../../../zigzag-instability.md), in addition to the longitudinal [Eckhaus instability](../../../../../eckhaus-instability.md). The fourth transverse [derivative](../../../../../derivative.md) and mixed [derivative](../../../../../derivative.md) in the square encode the critical-circle geometry.

One [complex amplitude](../../../../../complex-amplitude.md) still describes only a narrow cone of nearby roll orientations. Competing well-separated wavevectors require coupled [amplitude equations](../../../../../amplitude-equation.md); resonant triples can admit quadratic interactions and produce the [hexagonal convection amplitude equations](../../../../../hexagonal-convection-amplitude-equations.md) when the underlying sign symmetry allows them. Strong disorder, defect cores with large gradients, far-from-onset patterns, boundaries, mean flows and conserved fields may all lie outside the single-amplitude approximation. The [method of multiple scales](../../../../../method-of-multiple-scales.md) gives controlled leading behavior for small amplitudes and slow modulations, rather than a universal model of all two-dimensional pattern selection.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
