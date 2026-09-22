<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On a bosonic background, a [Killing spinor](../../../../../killing-spinor.md) is a nonzero spinor parameter that makes all fermionic [supersymmetry](../../../../../supersymmetry-split.md) variations vanish. It identifies an unbroken supersymmetry of the background; the number of independent solutions counts preserved supercharges. In simple ungauged [minimal four-dimensional supergravity](../../../../../minimal-four-dimensional-supergravity.md), with the gravitino set to zero, its equation is $\nabla_\mu\epsilon=0$ and the bosonic field equations are $R_{\mu\nu}=0$. In theories with additional fields or a cosmological deformation, the Killing-spinor equation instead uses the corresponding modified connection.

Use commuting spinors to form ordinary geometric bilinears, and orient the [Dirac current](../../../../../dirac-current.md) to the future with $\bar\epsilon=-\epsilon^\dagger\gamma^{\hat0}$ in mostly-plus signature. Since the spinor and gamma matrices are parallel,

$$
\nabla_\mu K_\nu=(\nabla_\mu\bar\epsilon)\gamma_\nu\epsilon+\bar\epsilon\gamma_\nu\nabla_\mu\epsilon=0.
$$

Thus $K$ is actually parallel, and in particular is a [Killing vector field](../../../../../killing-vector-field.md). In a local orthonormal frame,

$$
K^{\hat0}=\epsilon^\dagger\epsilon>0,\qquad
K^{\hat i}=\epsilon^\dagger\alpha^i\epsilon,\qquad\alpha^i=-\gamma^{\hat0}\gamma^{\hat i}.
$$

For every spatial unit vector $u$, $u_i\alpha^i$ is Hermitian and squares to one. Its eigenvalues are $\pm1$, so $|u_iK^i|\leq K^0$. Taking $u$ along the spatial current gives

$$
\boxed{K_\mu K^\mu=-(K^0)^2+|\mathbf K|^2\leq0.}
$$

A nonzero parallel spinor cannot vanish at an isolated point, so this causal [Dirac current](../../../../../dirac-current.md) is nonzero everywhere on a connected solution. Its squared norm is constant: it cannot alternate between timelike and null regions.

If $K$ is timelike, normalize its constant norm. Its parallel dual one-form is closed, and its orthogonal distribution is integrable. Adapted local coordinates put the metric in the product form

$$
ds^2=-dt^2+h_{ij}(x)dx^idx^j.
$$

The time independence follows because $K$ is Killing, and the unit lapse and zero cross terms follow from parallelism. The vacuum equations give $R_{ij}(h)=0$. In three dimensions the Riemann tensor is completely determined by the [Ricci tensor](../../../../../ricci-tensor.md) and its scalar contraction, so $h$ is flat. Therefore

$$
\boxed{\text{Every timelike-current solution is locally Minkowski spacetime.}}
$$

Constant spinors in its flat frame provide all local Killing spinors. Global identifications are possible only when they preserve a compatible [spin structure](../../../../../spin-structure.md) and the required spinors.

If $K$ is null, its parallelism first gives a Brinkmann coordinate system with $K=\partial_v$. The parallel-spinor condition further restricts the local spin holonomy to the stabilizer of that spinor. In four dimensions, for a nonzero Weyl component represented by $(1,0)^T$, its stabilizer in $SL(2,\mathbb C)$ is the upper-triangular group $\begin{pmatrix}1&b\\0&1\end{pmatrix}$, $b\in\mathbb C$: the two real null rotations, with no transverse rotation. Consequently the transverse frame is flat and the allowed curvature is of the wave type $R_{uiuj}$. Using the coordinate freedom to remove transverse cross terms gives the local [plane-fronted gravitational wave](../../../../../plane-fronted-gravitational-wave.md) form

$$
\boxed{ds^2=-2du\,dv+dx^2+dy^2+H(u,x,y)du^2,\qquad H_{xx}+H_{yy}=0.}
$$

Here $R_{uiuj}=-H_{ij}/2$ and the only potentially nonzero Ricci component is $R_{uu}=-(H_{xx}+H_{yy})/2$, so the last equation is exactly the vacuum equation. Conversely, in the coframe $e^+=du$, $e^-=dv-Hdu/2$, $e^i=dx^i$, the nonzero spin-connection matrices are proportional to $H_i\gamma^{+i}du$. Constant spinors with $\gamma^+\epsilon=0$ are therefore parallel. Every harmonic transverse profile, with arbitrary $u$ dependence, gives such a supersymmetric vacuum wave; the flat profile is included. This verifies both the form and sufficiency in the [parallel-spinor classification of vacuum four-geometries](../../../../../parallel-spinor-classification-of-vacuum-four-geometries.md).

There is a reality-condition subtlety in interpreting the branches. A single commuting four-dimensional Majorana spinor has a [null current of a commuting Majorana spinor](../../../../../null-current-of-a-commuting-majorana-spinor.md): its two-component representation gives $|\xi^\dagger\boldsymbol\sigma\xi|^2=(\xi^\dagger\xi)^2$. A timelike current can instead come from a Dirac Killing spinor or a sum of independent real-spinor currents. The conditional timelike classification above remains valid, but does not assert a generic timelike current for a single real Majorana parameter.

For the final question use constant sectional curvature $-1/a^2$, so $R_{\mu\nu}= -3g_{\mu\nu}/a^2$. The [spinor curvature identity](../../../../../spinor-curvature-identity.md) gives

$$
[\nabla_\mu,\nabla_\nu]\epsilon=-\frac1{2a^2}\gamma_{\mu\nu}\epsilon.
$$

Define the [Anti-de Sitter Killing-spinor connection](../../../../../anti-de-sitter-killing-spinor-connection.md) $\mathcal D_\mu=\nabla_\mu+\gamma_\mu/(2a)$. Since $\nabla_\mu\gamma_\nu=0$ and the connection is torsion-free,

$$
[\mathcal D_\mu,\mathcal D_\nu]
=-\frac1{2a^2}\gamma_{\mu\nu}+\frac1{4a^2}[\gamma_\mu,\gamma_\nu]=0.
$$

Thus the modified connection is flat. On a simply connected region, transport any initial spinor with this connection; flatness makes the result path independent and supplies actual nonzero solutions, not merely a necessary integrability condition. Hence

$$
\boxed{\nabla_\mu\epsilon+\frac1{2a}\gamma_\mu\epsilon=0}
$$

has a full local space of solutions on [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md), and globally on its universal cover. Global quotients require compatible spinor monodromy. These are Killing spinors of the cosmological deformation, not parallel-spinor vacua of the undeformed zero-cosmological-constant theory.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
