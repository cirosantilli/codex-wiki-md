<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a mass-normalized [galactic distribution function](../../../../../galactic-distribution-function.md) $F$, so that $\rho=\int F\,d^3v$ and $\rho\langle v_iv_j\rangle=\int v_iv_jF\,d^3v$. Multiplying the stationary [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) by $v_j$ and integrating over [velocity space](../../../../../velocity-space.md) gives

$$
\partial_i\int v_iv_jF\,d^3v-\Phi_{,i}\int v_j\partial_{v_i}F\,d^3v=0.
$$

Assume the [galactic distribution function](../../../../../galactic-distribution-function.md) decays sufficiently rapidly for the velocity boundary term to vanish. [Integration by parts](../../../../../integration-by-parts.md) then gives $\int v_j\partial_{v_i}F\,d^3v=-\delta_{ij}\rho$, and therefore the [Jeans equations](../../../../../jeans-equation.md) are

$$
\boxed{\partial_i(\rho\langle v_iv_j\rangle)=-\rho\Phi_{,j}.}
$$

The second moment includes both ordered motion and [velocity dispersion](../../../../../velocity-dispersion.md); no assumption of zero mean velocity was needed.

To obtain the [tensor virial theorem](../../../../../tensor-virial-theorem.md), multiply the $j$th [Jeans equation](../../../../../jeans-equation.md) by $x_i$ and integrate over position. For an isolated, finite system with a vanishing spatial surface term,

$$
-\int\rho\langle v_iv_j\rangle\,d^3x=-\int\rho x_i\Phi_{,j}\,d^3x=W_{ij}.
$$

Since the left side is $-2K_{ij}$, **$2K_{ij}+W_{ij}=0$**. This convention puts all stellar second moments into $K_{ij}$; it does not separate ordered and random [kinetic energies](../../../../../kinetic-energy.md).

For a self-gravitating system, the trace $W$ is the [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md). Indeed, symmetrizing the pair integral gives

$$
W=-\frac G2\iint\frac{\rho(\mathbf x)\rho(\mathbf x')}{|\mathbf x-\mathbf x'|}\,d^3x\,d^3x'=\frac12\int\rho\Phi\,d^3x.
$$

Thus the trace of the [tensor virial theorem](../../../../../tensor-virial-theorem.md) is $2K+W=0$, and the total energy obeys

$$
\boxed{E=K+W=-K=W/2.}
$$

These identities require self-gravity without an additional external potential or an omitted confining boundary pressure.

Let $\langle v_I^2\rangle$ now denote a mass-weighted average over the entire initial system. Then $K_I=M_I\langle v_I^2\rangle/2$. The [gravitational radius](../../../../../gravitational-radius.md) is defined by $R_I=-GM_I^2/W_I$, so the [virial theorem](../../../../../virial-theorem.md) immediately yields

$$
\boxed{E_I=-\frac12M_I\langle v_I^2\rangle=-\frac{GM_I^2}{2R_I}.}
$$

The [gravitational radius](../../../../../gravitational-radius.md) measures total binding energy, rather than a particular geometric edge or half-mass radius.

For the accreted systems define the mass-weighted internal mean-square speed by $M_A\langle v_A^2\rangle=\sum_sM_s\langle v_s^2\rangle$. If each satellite initially satisfies the [virial theorem](../../../../../virial-theorem.md), its internal energy contributes to $E_A=-M_A\langle v_A^2\rangle/2$. In [parabolic dry-merger energy accounting](../../../../../parabolic-dry-merger-energy-accounting.md), the orbital energy at large separation is zero. Assume a [dry galaxy merger](../../../../../dry-galaxy-merger.md), no loss of mass or energy through escaping stars, no external work, and a final relaxed system satisfying the [virial theorem](../../../../../virial-theorem.md). Then [conservation of energy](../../../../../conservation-of-energy.md) gives $E_F=E_I+E_A$ and $M_F=M_I+M_A$. Energy transferred by [Chandrasekhar dynamical friction](../../../../../chandrasekhar-dynamical-friction.md) remains part of the total energy under these assumptions. Consequently,

$$
E_F=-\frac12M_I\langle v_I^2\rangle(1+\epsilon\eta),\qquad \eta=\frac{M_A}{M_I},\quad\epsilon=\frac{\langle v_A^2\rangle}{\langle v_I^2\rangle}.
$$

Applying the final [virial theorem](../../../../../virial-theorem.md) and dividing by the initial relation gives

$$
\boxed{\frac{\langle v_F^2\rangle}{\langle v_I^2\rangle}=\frac{1+\epsilon\eta}{1+\eta},\qquad\frac{R_F}{R_I}=\frac{(1+\eta)^2}{1+\epsilon\eta}.}
$$

For a mass doubling, $\eta=1$. A merger of two identical equilibrated galaxies has $\epsilon=1$, hence **$R_F/R_I=2$**. For accretion through many [minor galaxy mergers](../../../../../minor-galaxy-merger.md) whose satellites have much smaller internal mean-square speeds, $\epsilon\ll1$, hence **$R_F/R_I\simeq4$**, tending to $4$ in the cold-satellite limit. Equivalently, nearly fixed total energy makes the [gravitational radius](../../../../../gravitational-radius.md) scale as $M^2$ during [cold minor-merger size growth](../../../../../cold-minor-merger-size-growth.md). Small satellite mass alone does not logically imply $\epsilon\ll1$: the factor four also requires this weak-binding assumption. Likewise, equal masses require comparable internal binding to give the factor two. These are the physical limits behind the two stated merger comparisons.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
