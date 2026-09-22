<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use target-space signature $(-,+,\ldots,+)$ and let a dot between target vectors denote contraction with the [Minkowski metric](../../../../../minkowski-metric.md). Varying the [string embedding map](../../../../../string-embedding-map.md) in the [Polyakov action](../../../../../polyakov-action.md), with periodic variations around the closed string, gives

$$
\delta_X I=\frac1{2\pi\alpha'}\int d^2\sigma\,\delta X_\mu\,\partial_a\big(\sqrt{-\gamma}\,\gamma^{ab}\partial_bX^\mu\big).
$$

Thus the embedding [equation of motion](../../../../../equation-of-motion.md) is

$$
\boxed{\partial_a\big(\sqrt{-\gamma}\,\gamma^{ab}\partial_bX^\mu\big)=0.}
$$

The independent [worldsheet metric](../../../../../worldsheet-metric.md) variation uses $\delta\sqrt{-\gamma}=-\tfrac12\sqrt{-\gamma}\gamma_{ab}\delta\gamma^{ab}$. It sets the [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) to zero:

$$
\boxed{\partial_aX\cdot\partial_bX-\frac12\gamma_{ab}\gamma^{cd}\partial_cX\cdot\partial_dX=0.}
$$

In [conformal gauge](../../../../../conformal-gauge.md), $\gamma_{ab}=e^{2\omega}\operatorname{diag}(-1,1)$, the Weyl factor cancels. Define worldsheet derivatives $\partial_\pm=(\partial_\tau\pm\partial_\sigma)/2$. The equations and [Virasoro constraints](../../../../../virasoro-constraint.md) reduce to

$$
\boxed{\partial_+\partial_-X^\mu=0,\qquad (\partial_+X)^2=(\partial_-X)^2=0.}
$$

Equivalently, $\ddot X-X''=0$, $\dot X\cdot X'=0$ and $\dot X^2+X'^2=0$. The free wave equation permits independent periodic left- and right-moving fields.

Take $0\le\sigma<2\pi$ and the uncompactified [closed-string mode expansion](../../../../../closed-string-mode-expansion.md)

$$
X^\mu=x^\mu+\alpha'p^\mu\tau+i\sqrt{\frac{\alpha'}2}\sum_{n\ne0}\frac1n\left(\alpha_n^\mu e^{-in(\tau-\sigma)}+\widetilde\alpha_n^\mu e^{-in(\tau+\sigma)}\right),
\qquad \alpha_0^\mu=\widetilde\alpha_0^\mu=\sqrt{\frac{\alpha'}2}p^\mu.
$$

The [Virasoro generators](../../../../../virasoro-generator.md) are the Fourier coefficients of the two quadratic [worldsheet stress tensors](../../../../../worldsheet-stress-energy-tensor.md). Their quantum expressions are

$$
L_n=\frac12\sum_m:\!\alpha_{n-m}\cdot\alpha_m\!:,
\qquad \widetilde L_n=\frac12\sum_m:\!\widetilde\alpha_{n-m}\cdot\widetilde\alpha_m\!:.
$$

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) are $[\alpha_m^\mu,\alpha_n^\nu]=m\eta^{\mu\nu}\delta_{m+n,0}$, with an identical tilded algebra and commuting chiral sectors. [Normal ordering](../../../../../normal-ordering.md) places annihilation modes to the right. It gives $L_0=\alpha'p^2/4+N$, where $N=\sum_{n>0}\alpha_{-n}\cdot\alpha_n$, and similarly on the other side. In [old covariant string quantization](../../../../../old-covariant-string-quantization.md), [physical string states](../../../../../physical-string-state.md) obey

$$
L_{n>0}|\Psi\rangle=\widetilde L_{n>0}|\Psi\rangle=0,
\qquad (L_0-a)|\Psi\rangle=(\widetilde L_0-a)|\Psi\rangle=0,
$$

modulo physical [null string states](../../../../../null-string-state.md). Negative generators are adjoint constraints on bras, not further annihilation conditions on the same ket. In critical [bosonic string theory](../../../../../bosonic-string-theory.md), $d=26$ and the [string intercept](../../../../../normal-ordering-constant-of-a-string.md) is $a=1$. These [closed-string physical-state Virasoro conditions](../../../../../closed-string-physical-state-virasoro-conditions.md) imply

$$
N=\widetilde N,\qquad M^2=-p^2=\frac4{\alpha'}(N-1).
$$

Thus the [massless first closed-string level](../../../../../massless-first-closed-string-level.md) has $N=\widetilde N=1$, and its general state is

$$
|\zeta,p\rangle=\zeta_{\mu\nu}\alpha_{-1}^\mu\widetilde\alpha_{-1}^\nu|0,p\rangle.
$$

To derive the [polarization tensor](../../../../../polarization-tensor.md) constraints, the oscillator algebra gives $[L_n,\alpha_m^\mu]=-m\alpha_{n+m}^\mu$. Applying $L_1$ to this state replaces $\alpha_{-1}^\mu$ by $\alpha_0^\mu$; the independent tilded condition replaces the other oscillator by $\widetilde\alpha_0^\nu$. All higher positive generators annihilate the state automatically. Therefore

$$
\boxed{p^2=0,\qquad p^\mu\zeta_{\mu\nu}=0,\qquad p^\nu\zeta_{\mu\nu}=0.}
$$

There is no condition that the tensor trace vanish: each chiral side has only one oscillator, so neither $L_2$ nor $\widetilde L_2$ imposes a trace condition. The [null-state quotient of a string](../../../../../null-state-quotient-of-a-string.md) also identifies

$$
\zeta_{\mu\nu}\sim\zeta_{\mu\nu}+p_\mu\xi_\nu+p_\nu\widetilde\xi_\mu,
\qquad p\cdot\xi=p\cdot\widetilde\xi=0.
$$

For example, $L_{-1}(\xi_\nu\widetilde\alpha_{-1}^\nu|0,p\rangle)$ is a momentum-longitudinal state with zero inner product against every transverse physical polarization. This explains the [string-state gauge redundancy](../../../../../string-state-gauge-redundancy.md), rather than merely counting covariant components. For an ordinary nonzero null momentum, choose a frame adapted to $p$. The constraints remove one null direction in each index, and these null-state identifications remove the remaining longitudinal directions. The representatives are then $\zeta_{ij}$, $i,j=1,\ldots,24$.

Decompose that transverse matrix into its symmetric trace-free part, antisymmetric part and trace. **They describe the [graviton](../../../../../graviton.md), [Kalb–Ramond field](../../../../../kalb-ramond-field.md) and [dilaton](../../../../../dilaton.md), respectively.** Their [particle polarization](../../../../../particle-polarization.md) counts are

$$
\boxed{\left(\frac{24\cdot25}{2}-1\right)+\frac{24\cdot23}{2}+1=299+276+1=576.}
$$

These are representations of the rotational part $SO(24)$ of the massless [little group](../../../../../little-group.md). The dilaton corresponds to the transverse trace; a covariant scalar polarization can be written proportional to $\eta_{\mu\nu}-p_\mu\ell_\nu-\ell_\mu p_\nu$, with $\ell^2=0$ and $p\cdot\ell=1$. It is transverse in both indices and has trace 24. The nonzero-momentum assumption is appropriate for propagating particle states; zero momentum requires separate treatment of gauge and background zero modes.

In a general background, these fields replace the flat-space free action by the [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md). A convenient Euclidean convention is

$$
\begin{aligned}
S_E[X,\gamma;G,B,\Phi]
={}&\frac1{4\pi\alpha'}\int d^2\sigma\,\sqrt\gamma\,\gamma^{ab}G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu\\
&+\frac{i}{4\pi\alpha'}\int d^2\sigma\,\epsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu
+\frac1{4\pi}\int d^2\sigma\,\sqrt\gamma\,\Phi(X)R^{(2)}.
\end{aligned}
$$

Here $\epsilon^{ab}$ is the orientation density; reversing its convention changes the displayed sign of the two-form coupling. The [metric tensor](../../../../../metric-tensor.md) is $G_{\mu\nu}=\eta_{\mu\nu}+h_{\mu\nu}+\cdots$, $B$ is the antisymmetric [Kalb–Ramond field](../../../../../kalb-ramond-field.md), and $\Phi$ is the [dilaton](../../../../../dilaton.md). Their worldsheet couplings reproduce the corresponding [massless closed-string vertex operators](../../../../../massless-closed-string-vertex-operator.md) when expanded about flat space. The [Polyakov path integral](../../../../../polyakov-path-integral.md) integrates $e^{-S_E}$ over embedding fields and metrics modulo [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md) and [Weyl transformations](../../../../../weyl-transformation.md); [gauge fixing](../../../../../gauge-fixing.md) supplies ghost determinants and moduli integrations. Quantum consistency of a general background additionally requires vanishing [sigma-model beta functions](../../../../../sigma-model-beta-function.md), not just insertion of arbitrary backgrounds into a free theory.

Finally, separate the constant dilaton mode, $\Phi=\Phi_0+\widehat\Phi$. By the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md), its action is

$$
S_{\Phi_0}=\frac{\Phi_0}{4\pi}\int\sqrt\gamma R^{(2)}=\Phi_0\chi(\Sigma).
$$

For a connected oriented surface of [genus](../../../../../genus-of-a-surface.md) $g$, its [Euler characteristic](../../../../../euler-characteristic.md) is $\chi=2-2g$. Defining the [string coupling](../../../../../string-coupling.md) by $g_s=e^{\Phi_0}$ gives

$$
\boxed{e^{-S_{\Phi_0}}=g_s^{-\chi}=g_s^{2g-2}.}
$$

Thus the [string genus expansion](../../../../../string-genus-expansion.md) is a topology sum with two extra powers of $g_s$ per handle. An amplitude with $n$ canonically normalized external closed-string vertices has the additional vertex normalization $g_s^n$, so its overall factor is $g_s^{2g-2+n}$. The curvature term, rather than a guessed coupling inserted at each internal interaction, supplies this dependence directly from the functional integral.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
