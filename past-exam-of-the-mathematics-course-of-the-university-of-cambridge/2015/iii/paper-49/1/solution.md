<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [Minkowski spacetime](../../../../../minkowski-spacetime.md) signature $(-,+,+,+)$ and a closed spatial parameter of period $2\pi$. Choose the future-directed branch with positive lapse $e$.

**Canonical dynamics and gauge freedom.** Variation of momentum and embedding in the [Nambu-Goto phase-space action](../../../../../nambu-goto-phase-space-action.md) gives

$$
\boxed{\dot X^m=eP^m+uX'^m,\qquad
\dot P_m=\partial_\sigma(eT^2X'_m+uP_m).}
$$

The [Lagrange multipliers](../../../../../lagrange-multiplier.md) impose the [Nambu–Goto phase-space constraints](../../../../../nambu-goto-phase-space-constraints.md) $P^2+T^2X'^2=0$ and $P\cdot X'=0$. These two [first-class constraints](../../../../../first-class-constraint.md) reflect freedom to relabel time and space on the same [string worldsheet](../../../../../worldsheet.md). The canonical [Hamiltonian](../../../../../hamiltonian.md) is a linear combination of constraints, with arbitrary multiplier functions. These functions specify a coordinate description rather than additional propagating fields. No explicit gauge transformation or Poisson-bracket calculation is required.

**Eliminating auxiliary variables.** Let $V=\dot X-uX'$. Eliminating momentum using $P=V/e$ leaves

$$
\mathcal L=\frac{V^2}{2e}-\frac{eT^2}{2}X'^2.
$$

On a patch with spacelike spatial tangent, variation of $u$ gives $V\cdot X'=0$, hence $u=(\dot X\cdot X')/X'^2$. For the [induced worldsheet metric](../../../../../induced-worldsheet-metric.md) $g_{ab}=\partial_aX\cdot\partial_bX$, this gives $V^2=\det g/X'^2$. Variation of $e$ then gives $e=\sqrt{-\det g}/(TX'^2)$ on the positive branch. Substitution yields

$$
\boxed{I_{\mathrm{NG}}=-T\int dt\,d\sigma\,\sqrt{-\det g}.}
$$

This is minus [string tension](../../../../../string-tension.md) times Lorentzian [worldsheet area](../../../../../worldsheet-area.md). Vary the area using $\delta\sqrt{-g}=\tfrac12\sqrt{-g}\,g^{ab}\delta g_{ab}$ and integrate by parts. The [Nambu–Goto equations of motion](../../../../../nambu-goto-equations-of-motion.md) are

$$
\boxed{\partial_a\!\left(\sqrt{-g}\,g^{ab}\partial_bX^m\right)=0.}
$$

The auxiliary-variable elimination and this metric form apply on nondegenerate timelike patches.

**Circular motion, length and [energy](../../../../../energy.md).** For the circular embedding, direct differentiation gives

$$
g_{tt}=-R^2\cos^2t,\qquad
g_{\sigma\sigma}=R^2\cos^2t,\qquad g_{t\sigma}=0.
$$

Away from collapse, $\sqrt{-g}\,g^{ab}=\operatorname{diag}(-1,1)$, so the equations become $\ddot X^m-X''^m=0$. The time and out-of-plane coordinates satisfy them immediately. For $Z=X^1+iX^2$, both $\ddot Z$ and $Z''$ are $-Z$. The relations $\dot X\cdot X'=0$ and $\dot X^2+X'^2=0$ verify the [Virasoro constraints](../../../../../virasoro-constraint.md). Equivalently, $e=1/T$, $u=0$, $P=T\dot X$ solve the phase-space equations and constraints at all times.

The ring stays in a fixed plane, with radius $R|\cos t|$. It contracts to a point and re-expands. Each labeled point moves radially with speed $|\sin t|$ in target time $X^0=Rt$. The geometric ring repeats after target-time interval $\pi R$, although the labels have then shifted by half a circumference. It is not rigidly rotating. Velocity is perpendicular to the tangent, so simultaneous spatial arclength is also the local [proper length](../../../../../proper-length.md) along the string. Its length and conserved [energy](../../../../../energy.md) are

$$
\boxed{L(t)=2\pi R|\cos t|,\qquad
E=\int_0^{2\pi}P^0\,d\sigma=2\pi TR.}
$$

Away from collapse, the same [energy](../../../../../energy.md) follows from $T\int dl/\sqrt{1-v^2}$. Increasing kinetic [energy](../../../../../energy.md) compensates the shrinking length. At collapse the induced metric degenerates; the area-form equation alone is undefined there. The regular phase-space solution supplies the continuation and the limiting constant [energy](../../../../../energy.md). This is a [pulsating circular string](../../../../../pulsating-circular-string.md).

**Endpoint variation.** For an [open string](../../../../../open-string.md), integration by parts produces the boundary term

$$
\delta I_{\mathrm{end}}=-\int dt\,
\left[(eT^2X'_m+uP_m)\delta X^m\right]_{\mathrm{ends}}.
$$

Its coefficient is the [open-string endpoint momentum flux](../../../../../open-string-endpoint-momentum-flux.md). Evaluate this ungauge-fixed variation in a boundary-adapted [temporal gauge for a string](../../../../../temporal-gauge-for-a-string.md) $X^0=t$. Then $X'^0=0$ and the time equation gives $P^0=1/e\ne0$. The free variation of time forces $uP_0=0$, hence $u=0$ at each end. Since $e$ is nonzero, the remaining spatial term requires

$$
\boxed{(\vec X'\cdot\delta\vec X)_{\mathrm{ends}}=0.}
$$

Free variation in every spatial direction gives $\vec X'=0$, and together with $X'^0=0$ gives the [free-end string boundary condition](../../../../../free-end-string-boundary-condition.md) $X'^m=0$. The general starting condition is the flux condition; the shift term should not be silently discarded before choosing the gauge.

**Target-space charges.** The [Noether charges](../../../../../noether-charge.md) for translations and [Lorentz transformations](../../../../../lorentz-transformation.md) are the [target-space Noether charges of a string](../../../../../target-space-noether-charges-of-a-string.md)

$$
\boxed{\mathcal P_m=\int P_m\,d\sigma,\qquad
\mathcal J_{mn}=\int(X_mP_n-X_nP_m)\,d\sigma.}
$$

Writing $F_m=eT^2X'_m+uP_m$, the canonical equations imply

$$
\dot{\mathcal P}_m=[F_m]_{\mathrm{ends}},\qquad
\dot{\mathcal J}_{mn}=[X_mF_n-X_nF_m]_{\mathrm{ends}}.
$$

For the second identity, antisymmetry cancels the $eP_mP_n$ terms. Integration by parts then cancels the $uX'P$ terms and the symmetric $eT^2X'_mX'_n$ terms. For free ends $F_m=0$ individually, so both charges are constant. In [conformal gauge](../../../../../conformal-gauge.md), the same result follows from $u=0$ and $X'^m=0$. Target-space [energy](../../../../../energy.md) is $-\mathcal P_0$.

Other possibilities fix selected spatial directions by [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), while leaving [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) in the permitted tangent directions. These mixed conditions describe endpoints on a [D-brane](../../../../../d-brane.md); the two ends can lie on different branes. Time stays free under the given assumption. Fixed supports may absorb momentum in their Dirichlet directions and break corresponding translations or Lorentz symmetries. More general force-law conditions require an additional boundary interaction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
