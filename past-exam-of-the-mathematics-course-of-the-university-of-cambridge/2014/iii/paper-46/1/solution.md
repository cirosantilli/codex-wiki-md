<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the mostly-plus [Minkowski metric](../../../../../minkowski-metric.md), and write $\approx$ for equality on the [constraint surface](../../../../../constraint-surface.md). Assume that the [mechanical constraints](../../../../../constraint-mechanics.md) are locally independent. They are [first-class constraints](../../../../../first-class-constraint.md) when

$$
\{\varphi_i,\varphi_j\}=C_{ij}{}^k(q,p)\varphi_k.
$$

Thus their [Poisson brackets](../../../../../poisson-bracket.md) vanish on the [constraint surface](../../../../../constraint-surface.md), and their [Hamiltonian](../../../../../hamiltonian.md) flows preserve that surface. The [structure functions of a constraint algebra](../../../../../structure-functions-of-a-constraint-algebra.md) $C_{ij}{}^k$ may depend on the [phase space](../../../../../phase-space.md) point. **The finite real span of the constraints is a [Lie algebra](../../../../../lie-algebra-split.md) if it closes with constant structure coefficients**, in a suitable choice of generators. The [Jacobi identity](../../../../../jacobi-identity.md) then gives the usual conditions on the [structure constants of a Lie algebra](../../../../../structure-constant-of-a-lie-algebra.md). With general structure functions the finite real span need not close, even though the [Poisson bracket](../../../../../poisson-bracket.md) of all smooth functions is itself a [Lie bracket](../../../../../lie-bracket.md).

To see the [gauge invariance](../../../../../gauge-invariance.md) directly, let $G=\epsilon^i(t)\varphi_i$ generate a [canonical gauge transformation](../../../../../canonical-gauge-transformation.md):

$$
\delta q^I=\{q^I,G\},\qquad
\delta p_I=\{p_I,G\},\qquad
\boxed{\delta\lambda^k=\dot\epsilon^k-\lambda^i\epsilon^jC_{ij}{}^k.}
$$

The variation of the [phase-space action](../../../../../phase-space-action.md) integrand is

$$
\delta(p_I\dot q^I-\lambda^i\varphi_i)
=\frac{d}{dt}(p_I\delta q^I-G)
+\left(\dot\epsilon^k-\delta\lambda^k-\lambda^i\epsilon^jC_{ij}{}^k\right)\varphi_k.
$$

The second term cancels without using the [equations of motion](../../../../../equation-of-motion.md). Taking $\epsilon^i$ to vanish at the temporal boundaries leaves the [action](../../../../../action.md) invariant. Arbitrary functions $\epsilon^i(t)$ therefore relate different descriptions of the same physical motion. This reasoning also works with structure functions; constant structure coefficients are only needed for the finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md) claim.

For a [closed string](../../../../../closed-string.md), choose $0\leq\sigma<2\pi$ and periodic fields. A convenient [Nambu-Goto phase-space action](../../../../../nambu-goto-phase-space-action.md) is

$$
I=\int dt\,d\sigma\left[P_m\dot X^m-\frac e2(P^2+T^2X'^2)-vP\cdot X'\right].
$$

Here $e$ and $v$ are [Lagrange multipliers](../../../../../lagrange-multiplier.md). The [Nambu–Goto phase-space constraints](../../../../../nambu-goto-phase-space-constraints.md) are $\mathcal H_0=(P^2+T^2X'^2)/2\approx0$ and $\mathcal H_1=P\cdot X'\approx0$, with canonical [Poisson brackets](../../../../../poisson-bracket.md)

$$
\{X^m(\sigma),P_n(\sigma')\}=\delta^m_n\delta_{2\pi}(\sigma-\sigma').
$$

Let $J_\pm^m=P^m\pm TX'^m$. Differentiating the periodic [Dirac delta function](../../../../../dirac-delta-function.md) gives

$$
\{P^m(\sigma),X'^n(\sigma')\}
=\eta^{mn}\partial_\sigma\delta_{2\pi}(\sigma-\sigma'),
\qquad
\{X'^m(\sigma),P^n(\sigma')\}
=\eta^{mn}\partial_\sigma\delta_{2\pi}(\sigma-\sigma').
$$

The opposite signs in $J_+$ and $J_-$ cancel these terms, so **$\{J_+^m(\sigma),J_-^n(\sigma')\}=0$**. Replace the original [constraints](../../../../../constraint-mechanics.md) by the equivalent chiral densities

$$
\mathcal H_\pm=\frac{J_\pm^2}{4T},\qquad
\mathcal H_0=T(\mathcal H_++\mathcal H_-),\qquad
\mathcal H_1=\mathcal H_+-\mathcal H_-.
$$

Their mixed [Poisson brackets](../../../../../poisson-bracket.md) vanish. Choose opposite Fourier orientations for the two sectors:

$$
L_n=\int_0^{2\pi}d\sigma\,e^{in\sigma}\mathcal H_+(\sigma),\qquad
\widetilde L_n=\int_0^{2\pi}d\sigma\,e^{-in\sigma}\mathcal H_-(\sigma).
$$

The [chiral constraint algebra of a closed string](../../../../../chiral-constraint-algebra-of-a-closed-string.md) is

$$
\boxed{\{L_m,L_n\}=-i(m-n)L_{m+n},\quad
\{\widetilde L_m,\widetilde L_n\}=-i(m-n)\widetilde L_{m+n},\quad
\{L_m,\widetilde L_n\}=0.}
$$

Each is the [Witt algebra](../../../../../witt-algebra.md): the [vector fields](../../../../../vector-field.md) $\ell_n=ie^{in\sigma}\partial_\sigma$ on a circle satisfy $[\ell_m,\ell_n]=(m-n)\ell_{m+n}$. Fourier expansion identifies each real algebra, with $L_n^*=L_{-n}$, with the [Lie algebra](../../../../../lie-algebra-split.md) of [vector fields](../../../../../vector-field.md) on the circle. The two commuting copies give **$\mathrm{Diff}_1\oplus\mathrm{Diff}_1$**, not a quantum central extension.

For an [open string](../../../../../open-string.md), allowed [boundary conditions](../../../../../boundary-condition.md) must remove the endpoint term in the variation of the [action](../../../../../action.md), consistently with the allowed endpoint variations. The spatial boundary term is

$$
\delta I\big|_{\partial\sigma}=-\int dt\,
\left[(eT^2X'_m+vP_m)\delta X^m\right]_{\sigma=a}^{\sigma=b}.
$$

It expresses the [open-string endpoint momentum flux](../../../../../open-string-endpoint-momentum-flux.md). In the [temporal gauge for a string](../../../../../temporal-gauge-for-a-string.md) $X^0=t$, take a boundary-adapted parametrization with $v=0$ at the ends. Fixing $X^i(t,a)=0$ gives $\delta X^i(t,a)=0$, a [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md). At the other end allow arbitrary spatial variations; for nonzero $e$ these require $X'^i(t,b)=0$, a [Neumann boundary condition](../../../../../neumann-boundary-condition.md). Also $X'^0=0$ in this [temporal gauge for a string](../../../../../temporal-gauge-for-a-string.md), so $X'^m(t,b)=0$. The [constraint](../../../../../constraint-mechanics.md) at this [free-end string boundary condition](../../../../../free-end-string-boundary-condition.md) reduces to $P^2=0$. Hamilton's equation $\dot X=eP+vX'$ consequently gives $\dot X^2=0$ there. Since $\dot X^0=1$, **the free endpoint has spatial speed one**. This is the [null motion of a free string endpoint](../../../../../null-motion-of-a-free-string-endpoint.md).

A [straight rotating string with one fixed endpoint](../../../../../straight-rotating-string-with-one-fixed-endpoint.md) supplies the required solution in at least two spatial dimensions. Set $e=1/T$, $v=0$, and

$$
\boxed{X^0=t,\qquad
\boldsymbol X(t,\sigma)=L\sin(\sigma/L)
\big(\cos(t/L),\sin(t/L),0,\ldots\big),\quad
0\leq\sigma\leq\frac{\pi L}{2}.}
$$

Take $P_m=T\dot X_m$. The [Hamilton's equations](../../../../../hamilton-s-equations.md) become $\ddot X=X''$, which holds because both second derivatives give $-\boldsymbol X/L^2$. The [Nambu–Goto phase-space constraints](../../../../../nambu-goto-phase-space-constraints.md) are satisfied by

$$
\dot X\cdot X'=0,\qquad
\dot X^2+X'^2=-1+\sin^2(\sigma/L)+\cos^2(\sigma/L)=0.
$$

The endpoint at $\sigma=0$ stays at the origin, while $X'=0$ at $\sigma=\pi L/2$ and the endpoint moves around a circle of radius $L$ with [angular speed](../../../../../angular-speed.md) $1/L$. At each time the whole string lies on a straight radial segment. Its spatial [proper length](../../../../../proper-length.md) is

$$
\int_0^{\pi L/2}|\boldsymbol X'|\,d\sigma
=\int_0^{\pi L/2}\cos(\sigma/L)\,d\sigma=L.
$$

The [velocity](../../../../../velocity.md) is everywhere perpendicular to the segment, so this also equals the sum of local rest-frame lengths. The induced [worldsheet metric](../../../../../worldsheet-metric.md) becomes degenerate at the null free endpoint, as expected for the limiting free-end solution.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
