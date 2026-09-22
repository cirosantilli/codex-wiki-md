# Virial theorem

↑ **Parent:** [Classical mechanics](classical-mechanics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virial_theorem)

The virial theorem relates the [average value of a function](average-value-of-a-function.md) along a trajectory to the [forces](force.md) that bind it. For an [isolated system](isolated-system.md) of particles interacting through [Newtonian gravitational potential energy](newtonian-gravitational-potential-energy.md), it gives $2\langle K\rangle+\langle U\rangle=0$: the average [kinetic energy](kinetic-energy.md) is half the magnitude of the average negative [potential energy](potential-energy.md). An eccentric [Kepler orbit](kepler-orbit.md) makes the distinction vivid: [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md) vary throughout the [orbit](orbit-dynamical-system.md), although their sum is constant. The relation concerns their [time](time-in-physics.md) averages, rather than their values at every instant. It underlies the [virial mass estimate](virial-mass-estimate.md) and the [negative heat capacity of a virialized gravitational system](negative-heat-capacity-of-a-virialized-gravitational-system.md).

Use constant positive particle [masses](mass.md) $m_i$, [positions](position.md) $\mathbf r_i$, mechanical [momenta](momentum.md) $\mathbf p_i=m_i\dot{\mathbf r}_i$, and total [kinetic energy](kinetic-energy.md) $K=\sum_i\mathbf p_i^2/(2m_i)$. The auxiliary quantity $G(t)$ is a sum of [dot products](dot-product.md), not the [gravitational constant](gravitational-constant.md), which we denote here by $G_{\!N}$:

$$
G(t)=\sum_i\mathbf p_i(t)\cdot\mathbf r_i(t),\qquad
\langle A\rangle_T=\frac1T\int_0^T A(t)\,dt,\qquad
2\langle K\rangle_T+\left\langle\sum_i\mathbf r_i\cdot\mathbf F_i\right\rangle_T
=\frac{G(T)-G(0)}{T}.
$$

This finite-$T$ identity is exact wherever [Newton's second law](newton-s-second-law.md) holds along a regular trajectory; $\mathbf F_i$ must include every [force](force.md). The endpoint term is what a finite observation window leaves behind. For the infinite-[time](time-in-physics.md) theorem, suppose the averages on the left exist and $(G(T)-G(0))/T\to0$. A sufficient condition is uniformly bounded [positions](position.md) and [velocities](velocity.md) for finitely many particles. More generally $G(T)=o(T)$ suffices, even without those individual bounds. Bounded [positions](position.md) alone do not supply a bound on [momenta](momentum.md), especially near a singular [potential energy](potential-energy.md); nor does a small endpoint term prove [thermodynamic equilibrium](thermodynamic-equilibrium.md). Periodic motion with $G(T)=G(0)$ gives the identity without an endpoint term at that finite $T$. For an [isolated system](isolated-system.md), use an inertial [centre of mass](center-of-mass.md) frame so translational drift does not contribute bulk [kinetic energy](kinetic-energy.md).[Cosmology by David Tong, §1.4.3, “The Virial Theorem and Galaxy Clusters”: bounded positions and velocities, existence of averages, equation (1.74) and endpoint limit](cosmology-by-david-tong/1-the-expanding-universe.md)

For a differentiable [potential energy](potential-energy.md) that is a [homogeneous function](homogeneous-function.md) of degree $q$, choose its additive constant so that the scaling law really holds. With [conservative forces](conservative-force.md), the [Euler theorem for homogeneous functions](euler-theorem-for-homogeneous-functions.md) gives

$$
U(\lambda\mathbf r_1,\ldots,\lambda\mathbf r_N)=\lambda^qU(\mathbf r_1,\ldots,\mathbf r_N),\qquad
\sum_i\mathbf r_i\cdot\mathbf F_i=-qU,\qquad
2\langle K\rangle_T-q\langle U\rangle_T=\frac{G(T)-G(0)}T.
$$

Thus a [harmonic oscillator](simple-harmonic-motion.md) has $q=2$ and $\langle K\rangle=\langle U\rangle$. An [isolated system](isolated-system.md) with [Newtonian gravitational potential energy](newtonian-gravitational-potential-energy.md) has

$$
U=-G_{\!N}\sum_{i<j}\frac{m_im_j}{|\mathbf r_i-\mathbf r_j|},\qquad q=-1,\qquad
2\langle K\rangle+\langle U\rangle=0,\qquad
E=\langle K\rangle+\langle U\rangle=-\langle K\rangle.
$$

Each interacting pair occurs once, and $U=0$ at infinite separation. Here the total [energy](energy.md) $E=K+U$ is conserved. An external field or a mixture of different scaling powers requires its own [force](force.md) term; one cannot assign the whole [potential energy](potential-energy.md) a single degree $q$. The [virial theorem for a homogeneous pair potential](virial-theorem-for-a-homogeneous-pair-potential.md) states the corresponding general [energy](energy.md) relation.

**Table of contents**

- [Virial theorem on a Kepler ellipse](virial-theorem-on-a-kepler-ellipse.md)
- [Virial mass estimate](virial-mass-estimate.md)
- [Boundary-pressure correction to the virial theorem](boundary-pressure-correction-to-the-virial-theorem.md)
- [Virial theorem derivation and history](virial-theorem-derivation-and-history.md)
- [Virial mean escape speed](virial-mean-escape-speed.md)
- [Virial theorem for a homogeneous pair potential](virial-theorem-for-a-homogeneous-pair-potential.md)
- [Negative heat capacity of a virialized gravitational system](negative-heat-capacity-of-a-virialized-gravitational-system.md)
- [Radiative energy of virialized gravitational collapse](radiative-energy-of-virialized-gravitational-collapse.md)
- [Virial equilibrium](virial-equilibrium.md)
- [Positive-energy linear diameter growth](positive-energy-linear-diameter-growth.md)
- [Pairwise moment-of-inertia identity](pairwise-moment-of-inertia-identity.md)
  - [Maximum-separation inertia bounds](maximum-separation-inertia-bounds.md)
- [Virial temperature](virial-temperature.md)
  - [Virial mass contours in a cooling diagram](virial-mass-contours-in-a-cooling-diagram.md)
- [Fixed-energy virial constraint between steady states](fixed-energy-virial-constraint-between-steady-states.md)
- [Gravitational radius](gravitational-radius.md)
  - [Gravitational rms escape and collapse speeds](gravitational-rms-escape-and-collapse-speeds.md)

## ↑ Ancestors (4)

1. [Classical mechanics](classical-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (69)

- [Boundary virial term of a singular isothermal sphere](boundary-virial-term-of-a-singular-isothermal-sphere.md)
- [Cluster temperature function normalization](cluster-temperature-function-normalization.md)
- [Cluster velocity-dispersion mass estimate](cluster-velocity-dispersion-mass-estimate.md)
- [Cold minor-merger size growth](cold-minor-merger-size-growth.md)
- [Dry galaxy merger](dry-galaxy-merger.md)
- [Effective equation of state of an oscillating scalar field](effective-equation-of-state-of-an-oscillating-scalar-field.md)
- [Einstein-de Sitter virial overdensity](einstein-de-sitter-virial-overdensity.md)
- [Global projected virial estimate of a mass-to-light ratio](global-projected-virial-estimate-of-a-mass-to-light-ratio.md)
- [Gravitational rms escape and collapse speeds](gravitational-rms-escape-and-collapse-speeds.md)
- [Local virial relation of the hypervirial model](local-virial-relation-of-the-hypervirial-model.md)
- [Minimum virial-radius ratio with positive cosmological constant](minimum-virial-radius-ratio-with-positive-cosmological-constant.md)
- [Parabolic dry-merger energy accounting](parabolic-dry-merger-energy-accounting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-44/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-44/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-45/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-45/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-45/3/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-62/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-66/4/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-66/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-66/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-67/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-73/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/15a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-61/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-69/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-72/3/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-62/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-62/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-65/3/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-60/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-60/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-60/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-56/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-58/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-61/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-62/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-320/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-320/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-320/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-320/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/13c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/13c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-320/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-320/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-346/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-4/9b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-4/9b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-310/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-315/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-320/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-346/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-349/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/9d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/9d/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-347/2/a/solution.md)
- [Quadrupole strain scaling of a weak self-gravitating source](quadrupole-strain-scaling-of-a-weak-self-gravitating-source.md)
- [Radiative energy of virialized gravitational collapse](radiative-energy-of-virialized-gravitational-collapse.md)
- [Uniform-sphere collapse with a cosmological constant](uniform-sphere-collapse-with-a-cosmological-constant.md)
- [Virial contraction under stellar evaporation](virial-contraction-under-stellar-evaporation.md)
- [Virial equilibrium](virial-equilibrium.md)
- [Virial mean escape speed](virial-mean-escape-speed.md)
- [Virial radius from turnaround energy](virial-radius-from-turnaround-energy.md)
- [Virial temperature](virial-temperature.md)
- [Virial theorem for a homogeneous pair potential](virial-theorem-for-a-homogeneous-pair-potential.md)
