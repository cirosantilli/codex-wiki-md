<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Actions and equations.** Use a mostly-plus [Minkowski metric](../../../../../minkowski-metric.md) and define the [induced worldsheet metric](../../../../../induced-worldsheet-metric.md) $h_{ab}=\partial_aX\cdot\partial_bX$. For a nondegenerate timelike [worldsheet](../../../../../worldsheet.md), the [Nambu–Goto action](../../../../../nambu-goto-action.md) is

$$
S_{\mathrm{NG}}=-T\int d^2\sigma\sqrt{-\det h}.
$$

Varying the independent metric in the [Polyakov action](../../../../../polyakov-action.md) sets its [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md) to zero:

$$
h_{ab}-\frac12\gamma_{ab}\gamma^{cd}h_{cd}=0.
$$

In two dimensions this says $h_{ab}=\Omega^2\gamma_{ab}$ for a positive local factor. The factor drops out of $\sqrt{-\gamma}\gamma^{ab}$, and substitution gives the [Nambu–Goto action](../../../../../nambu-goto-action.md). Conversely, any nondegenerate induced metric solves the auxiliary-metric equation up to a [Weyl transformation](../../../../../weyl-transformation.md). This [classical equivalence of Polyakov and Nambu–Goto actions](../../../../../classical-equivalence-of-polyakov-and-nambu-goto-actions.md) is a statement about classical embeddings; quantum equivalence additionally requires treatment of the metric measure and anomaly.

Variation of $X^m$ in the metric action, followed by elimination of $\gamma$, gives the [Nambu–Goto equations of motion](../../../../../nambu-goto-equations-of-motion.md)

$$
\boxed{\partial_a\!\left(\sqrt{-h}\,h^{ab}\partial_bX^m\right)=0.}
$$

A closed string has periodic $X$ and no spatial endpoint variation.

For a background metric $G$, [Kalb–Ramond field](../../../../../kalb-ramond-field.md) $b$, and [dilaton](../../../../../dilaton.md) $\Phi$, one consistent Lorentzian convention is

$$
S_L=-\frac1{4\pi\alpha'}\int d^2\sigma\sqrt{-\gamma}\,
\gamma^{ab}G_{mn}(X)\partial_aX^m\partial_bX^n
+\frac1{4\pi\alpha'}\int d^2\sigma\,\epsilon^{ab}b_{mn}(X)\partial_aX^m\partial_bX^n
-\frac1{4\pi}\int d^2\sigma\sqrt{-\gamma}\,\Phi(X)R^{(2)},
\qquad T=\frac1{2\pi\alpha'}.
$$

The orientation fixes the two-form sign; here the Lorentzian curvature convention is chosen so Wick rotation gives the positive Euclidean dilaton term $S_{E,\Phi}=\int\sqrt\gamma\Phi R^{(2)}/(4\pi)$. This avoids hiding the convention in the topology argument. For constant vacuum value $\Phi_0$, the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives $S_{E,\Phi}=\Phi_0\chi$. A connected closed oriented surface of genus $g$ has [Euler characteristic](../../../../../euler-characteristic.md) $\chi=2-2g$, so

$$
\boxed{e^{-S_{E,\Phi}}=e^{-\Phi_0(2-2g)}
=g_s^{2g-2},\qquad g_s=e^{\Phi_0}.}
$$

The connected vacuum amplitude has a [string genus expansion](../../../../../string-genus-expansion.md) $\sum_{g\ge0}g_s^{2g-2}\mathcal A_g$; disconnected vacuum diagrams exponentiate the connected sum. Each additional handle supplies a factor $g_s^2$. This is [dilaton Euler-characteristic weighting](../../../../../dilaton-euler-characteristic-weighting.md).

**The rotating circle.** For the specified embedding, the squared spatial speed and tangent length are both $1/2$, and their spatial inner product is zero. Including $X^0=t$ therefore gives

$$
\boxed{h_{ab}=\begin{pmatrix}-1/2&0\\0&1/2\end{pmatrix},\qquad
\sqrt{-h}=1/2.}
$$

The metric is constant. Its equation reduces to $\ddot X-X''=0$, satisfied by the left- and right-moving trigonometric components and the linear time component. On a constant-time slice with $0\le\sigma<2\pi$, the [proper length of a string](../../../../../proper-length-of-a-string.md) is

$$
\boxed{L=\int_0^{2\pi}\sqrt{h_{\sigma\sigma}}\,d\sigma
=\sqrt2\pi.}
$$

It is time-independent.

Let $R(\theta)$ be an ordinary two-dimensional rotation matrix. Rotate the first coordinate pair by $R(t)$ and the second by $R(-t)$. In these time-dependent Cartesian coordinates both pairs become $(\cos\sigma,\sin\sigma)/2$. A further fixed orthogonal change of basis gives

$$
Y_1=\frac{X_{\mathrm{rot}}^1+X_{\mathrm{rot}}^3}{\sqrt2}
=\frac{\cos\sigma}{\sqrt2},\qquad
Y_2=\frac{X_{\mathrm{rot}}^2+X_{\mathrm{rot}}^4}{\sqrt2}
=\frac{\sin\sigma}{\sqrt2},\qquad Y_3=Y_4=0.
$$

Thus every spatial slice is a planar circle of radius $1/\sqrt2$; its plane rotates in the ambient four-space. This is a [rigid circular string in four spatial dimensions](../../../../../rigid-circular-string-in-four-spatial-dimensions.md), not a pulsating circle. The rotating axes establish its spatial shape, not a transformation to an inertial spacetime frame.

The momentum density obtained from the [Nambu–Goto action](../../../../../nambu-goto-action.md) is $P_m=-T\sqrt{-h}\,h^{ta}\partial_aX_m$. Here $P_0=-T$, hence the conserved target-space energy is

$$
\boxed{E=-\int_0^{2\pi}P_0\,d\sigma=2\pi T=\sqrt2\,TL.}
$$

The material velocity is transverse to the tangent and has magnitude $1/\sqrt2$. Its Lorentz factor is $\sqrt2$, so the excess over $TL$ is kinetic energy. The spatial circle being stationary in rotating axes does not eliminate this energy.

**[Constraints](../../../../../constraint-mechanics.md) and endpoints.** Varying the multipliers in the [Nambu-Goto phase-space action](../../../../../nambu-goto-phase-space-action.md) imposes

$$
C=\frac12(P^2+T^2X'^2)=0,\qquad D=P\cdot X'=0.
$$

These are [first-class constraints](../../../../../first-class-constraint.md) generating normal and tangential [worldsheet diffeomorphisms](../../../../../worldsheet-diffeomorphism.md). They remove the two longitudinal embedding degrees of freedom; they are not extra physical force laws. Hamilton's equations are

$$
\boxed{\dot X^m=eP^m+uX'^m,\qquad
\dot P_m=(eT^2X'_m+uP_m)'.}
$$

For an open string, integration by parts leaves the spatial boundary variation

$$
\delta S_{\mathrm{end}}=-\int dt\,
\left[(eT^2X'_m+uP_m)\delta X^m\right]_{\sigma=0}^{\sigma=\pi}.
$$

Allowed [variational open-string boundary conditions](../../../../../variational-open-string-boundary-conditions.md) must make this vanish for every permitted endpoint displacement, and be preserved by the evolution. The bracketed expression is the [open-string endpoint momentum flux](../../../../../open-string-endpoint-momentum-flux.md). For free displacements, set that flux to zero. In a boundary-preserving gauge with $u=0$ and finite nonzero $e$, this is the [Neumann boundary condition](../../../../../neumann-boundary-condition.md) $X'^m=0$ at each end. This shows that [free-end string boundary conditions](../../../../../free-end-string-boundary-condition.md) are consistent.

At such an end, $C=0$ gives $P^2=0$, and $\dot X=eP$ gives $\dot X^2=0$. For a nontrivial endpoint trajectory with nonzero time velocity, its spatial speed is therefore one. This [null motion of a free string endpoint](../../../../../null-motion-of-a-free-string-endpoint.md) follows from the boundary condition together with the [constraints](../../../../../constraint-mechanics.md), not merely from the bulk wave equation. The induced metric may degenerate right at a free end; the result is understood as the endpoint limit or in the Polyakov description.

For a fixed spatial $p$-plane, split coordinates into $X^A$ along its $(p+1)$-dimensional worldvolume, including time, and $X^i$ transverse to it. Set $X'^A=0$ and $X^i=y^i$ at the ends. Tangential variations are free and their momentum flux vanishes; normal variations vanish, so their flux need not vanish. Evolution preserves the fixed normal values with $P^i=0$ at the boundary in the same gauge. These mixed [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) and [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) consistently restrict the endpoint worldlines to the plane.

The massless open-string excitations then separate into a gauge vector along the worldvolume and transverse [scalar fields](../../../../../scalar-field.md). A scalar displacement changes the corresponding $y^i$; its interpretation is a fluctuation of the plane's embedding. These [worldvolume fields from open-string massless states](../../../../../worldvolume-fields-from-open-string-massless-states.md) support the interpretation as a dynamical planar [D-brane](../../../../../d-brane.md). In the bosonic theory the still lower ground state is a [tachyon](../../../../../tachyon.md), indicating an unstable brane; the interpretation does not require pretending that this [tachyon](../../../../../tachyon.md) is a stable massless field. Appropriate superstring sectors can remove that instability.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
