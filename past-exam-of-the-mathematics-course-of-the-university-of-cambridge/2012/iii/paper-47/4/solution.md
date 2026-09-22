<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [instanton](../../../../../instanton.md) describes a finite-action trajectory in imaginary time that crosses between classical vacua. It accounts for [quantum tunnelling](../../../../../quantum-tunnelling.md) effects exponentially small in $\hbar$, beyond an ordinary power series around one minimum. A symmetric double well makes the connection between the [Euclidean path integral](../../../../../euclidean-path-integral.md), fluctuation theory and the low-energy spectrum particularly explicit.

For a particle of [mass](../../../../../mass.md) $\mu$, use a [Wick rotation](../../../../../wick-rotation.md) $t=-i\tau$ in the kernel. The [Euclidean action](../../../../../euclidean-action.md) and its classical equation are

$$
S_E[q]=\int d\tau\left[\tfrac12\mu\dot q^2+V(q)\right],\qquad \mu\ddot q=V'(q).
$$

The latter is Newtonian motion in the inverted potential $-V$. Subtract the common minimum energy so $V(\pm a)=0$. A finite-action path approaching $\pm a$ at infinite Euclidean times has conserved Euclidean energy $\mu\dot q^2/2-V=0$. Therefore

$$
\dot q=\pm\sqrt{2V(q)/\mu},\qquad S_I=\int_{-a}^a\sqrt{2\mu V(q)}dq.
$$

This gives both the classical trajectory by a quadrature and its tunnelling exponent. The plus solution is the [instanton](../../../../../instanton.md); reversal is the [anti-instanton](../../../../../anti-instanton.md). A single crossing has action $S_I$, not $2S_I$, although a periodic closed path necessarily has equal numbers of crossings in both directions.

**An explicit double well.** Take $V(q)=\mu\omega^2(q^2-a^2)^2/(8a^2)$, whose local harmonic frequency at either minimum is $\omega$. Integrating the zero-energy equation gives the [quartic double-well instanton](../../../../../quartic-double-well-instanton.md)

$$
\boxed{q_I(\tau)=a\tanh[\omega(\tau-\tau_0)/2],\qquad S_I=2\mu\omega a^2/3.}
$$

The arbitrary center $\tau_0$ is a [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md). The tunnelling regime is $S_I/\hbar\gg1$, so the crossing width $\omega^{-1}$ is short compared with the typical separation between rare crossings.

The exponential alone does not give a dimensionally complete amplitude. Expand $q=q_I+\eta$; the quadratic [Euclidean action](../../../../../euclidean-action.md) is $\mu\int\eta L_I\eta\,d\tau/2$, where

$$
L_I=-\partial_\tau^2+\omega^2\left[1-\tfrac32\operatorname{sech}^2\frac{\omega(\tau-\tau_0)}2\right],\qquad L_0=-\partial_\tau^2+\omega^2.
$$

The derivative $\dot q_I$ is a normalizable translation [instanton translation zero mode](../../../../../instanton-translation-zero-mode.md). The factorization of this one-dimensional fluctuation operator shows it has no negative modes. In $z=\omega(\tau-\tau_0)/2$, its two discrete eigenfunctions are proportional to $\operatorname{sech}^2z$ and $\operatorname{sech}z\tanh z$, with eigenvalues zero and $3\omega^2/4$; the continuum begins at $\omega^2$. Treating its zero eigenvalue as an ordinary [Gaussian integral](../../../../../gaussian-integral.md) would give a divergent determinant. Instead integrate over $\tau_0$: since $\mu\int\dot q_I^2d\tau=S_I$, the Jacobian supplies $\sqrt{S_I/(2\pi\hbar)}d\tau_0$. The nonzero fluctuations supply the determinant ratio. With common endpoint regularization,

$$
\boxed{K=\sqrt{\frac{S_I}{2\pi\hbar}}\left[\frac{\det L_0}{\det' L_I}\right]^{1/2},\qquad \kappa=K e^{-S_I/\hbar}.}
$$

This is the [instanton fluctuation prefactor](../../../../../instanton-fluctuation-prefactor.md), with $K$ and $\kappa$ having frequency units. The prime omits precisely the translation mode.

For this quartic potential the determinant can be evaluated explicitly. Set $z=\omega(\tau-\tau_0)/2$ and add a small positive spectral regulator $\varepsilon$ to both operators. With $r=2\sqrt{1+\varepsilon/\omega^2}$, the dimensionless operator is $-\partial_z^2+r^2-6\operatorname{sech}^2z$. Applying successively $-\partial_z+\tanh z$ and $-\partial_z+2\tanh z$ to the free decaying solution $e^{-rz}$, and normalizing at $z\to+\infty$, gives a growing coefficient at $z\to-\infty$ equal to $(r-1)(r-2)/[(r+1)(r+2)]$. The common Dirichlet [functional determinant](../../../../../functional-determinant.md) ratio has this coefficient. Hence the [quartic double-well fluctuation determinant](../../../../../quartic-double-well-fluctuation-determinant.md) is

$$
\frac{\det(L_I+\varepsilon)}{\det(L_0+\varepsilon)}=\frac{(r-1)(r-2)}{(r+1)(r+2)}=\frac{\varepsilon}{12\omega^2}+O(\varepsilon^2),\qquad
\boxed{\frac{\det' L_I}{\det L_0}=\frac1{12\omega^2},\quad K=\omega\sqrt{\frac{6S_I}{\pi\hbar}}.}
$$

The frequency factor cannot be discarded when deleting the zero eigenvalue.

**Summing rare crossings.** Consider Euclidean duration $T$ much longer than a crossing width. In the [dilute instanton gas](../../../../../dilute-instanton-gas.md), $n$ ordered centers have integration volume $T^n/n!$, and the amplitude per crossing is $\kappa$. Starting in the left well, directions alternate: an even number returns to the left well, and an odd number ends in the right well. If $E_{\rm well}=\hbar\omega/2+$ local anharmonic corrections, the leading kernels, with a common endpoint normalization $\mathcal A$, are

$$
\boxed{G_{LL}(T)\simeq\mathcal A e^{-E_{\rm well}T/\hbar}\cosh(\kappa T),\qquad G_{RL}(T)\simeq\mathcal A e^{-E_{\rm well}T/\hbar}\sinh(\kappa T).}
$$

The even/odd sums must not be replaced by counting all possible crossing directions independently. Comparing their exponential components with the spectral representation gives

$$
\boxed{E_{\rm even}=E_{\rm well}-\hbar\kappa,\quad E_{\rm odd}=E_{\rm well}+\hbar\kappa,\quad \Delta E=2\hbar K e^{-S_I/\hbar}.}
$$

For the quartic example, $\Delta E=2\hbar\omega\sqrt{6S_I/(\pi\hbar)}e^{-S_I/\hbar}$ to leading semiclassical order. This is the [double-well tunneling splitting](../../../../../double-well-tunneling-splitting.md): the even state is lower because the symmetric [wavefunction](../../../../../wave-function.md) has no node. The equivalent low-energy [Hamiltonian](../../../../../hamiltonian.md) in localized left/right states is $E_{\rm well}I-\hbar\kappa\sigma_x$. An initially localized state tunnels coherently, with probability $\sin^2(\Delta E\,t/(2\hbar))$ of occupying the other well. Tunnelling does not imply irreversible decay in this closed symmetric system.

The [instanton](../../../../../instanton.md) approach thus yields the same leading forbidden-region action as the [WKB approximation](../../../../../wkb-approximation.md), while identifying the zero-mode measure, fluctuation normalization and multiple tunnelling events systematically. Perturbation theory about either separate minimum cannot generate $e^{-S_I/\hbar}$. Multi-instanton interactions and higher-loop fluctuations correct the leading dilute-gas result; at finite temperature one instead uses periodic Euclidean boundary conditions, whose saddles may differ when the period is comparable to the crossing width. A false-vacuum bounce returning to the same metastable minimum has a negative fluctuation mode and describes a decay rate. It should not be confused with the stable-vacuum connecting [instanton](../../../../../instanton.md) above, which has a translation zero mode but no negative mode.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
