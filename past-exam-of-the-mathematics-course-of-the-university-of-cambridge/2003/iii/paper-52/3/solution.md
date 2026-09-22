<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Derrick scaling](../../../../../derrick-scaling.md) variation changes a configuration's size without changing its topological sector. Use $U_L(\mathbf x)=U(\mathbf x/L)$, so $L>1$ expands the configuration. An integrated nonnegative term homogeneous in $s$ spatial derivatives scales as $L^{d-s}E_s$. For a scalar gradient-plus-potential energy, for example,

$$
E(L)=L^{d-2}E_2+L^dE_0.
$$

A static solution is a stationary point of the full [energy functional](../../../../../energy-functional.md), so it must in particular satisfy $E'(1)=0$. In this example the [Derrick virial identity](../../../../../derrick-virial-identity.md) is $(d-2)E_2+dE_0=0$. If both energies are nonnegative and the coefficients cannot balance, a nontrivial localized static solution is impossible. If balance is possible, it fixes relations among energy contributions and may select a characteristic size. A negative $E''(1)$ proves an instability under size changes; a positive second derivative gives stability only against that one deformation. **Passing the scale test is a necessary condition, not an existence theorem or a proof of full stability.** It does not directly rule out time-dependent or charge-constrained solitons outside the static variational problem.

For the specified model, each spatial current is anti-Hermitian: differentiating $UU^\dagger=1$ gives $R_i^\dagger=-R_i$. Thus $-\operatorname{Tr}(R_i^2)$ is nonnegative, and the static energy of the [nonlinear sigma model](../../../../../nonlinear-sigma-model.md) is

$$
E_2=-\frac12\int_{\mathbb R^d}\operatorname{Tr}(R_iR_i)\,d^dx\ge0.
$$

The boundary condition $U\to1_2$ identifies spatial infinity to one point, so [one-point compactification](../../../../../alexandroff-extension.md) turns the field into a based map $S^d\to SU(2)$. By [SU(2) as the three-sphere](../../../../../su-2-as-the-three-sphere.md), its sectors are classified by the [homotopy group](../../../../../homotopy-group.md) $\pi_d(S^3)$. In particular,

$$
\pi_1(S^3)=0,\qquad\pi_2(S^3)=0,\qquad\pi_3(S^3)=\mathbb Z.
$$

There is no corresponding topological protection in one or two spatial dimensions. In three dimensions there is an integer [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md), the usual [topological baryon number in the Skyrme model](../../../../../topological-baryon-number-in-the-skyrme-model.md) when the same field is interpreted in that theory. With a compatible orientation convention it can be written

$$
B=-\frac1{24\pi^2}\int\epsilon_{ijk}\operatorname{Tr}(R_iR_jR_k)\,d^3x.
$$

Conjugation from the left current to the right current preserves the trace in this formula. Higher dimensions are governed by their corresponding homotopy groups, which need not all be trivial; no assumption of their triviality is needed in the scaling obstruction below.

For the pure sigma model, $E(L)=L^{d-2}E_2$, so stationarity requires $(d-2)E_2=0$. In every $d\ne2$ a finite-energy nonconstant static solution is excluded by [Derrick scaling](../../../../../derrick-scaling.md). In $d=1$ spreading lowers its energy; in $d>2$ shrinking lowers it. In particular, a degree-carrying three-dimensional sigma configuration can collapse toward zero size and energy within its sector, with a singular limiting field. The topological charge prevents smooth unwinding, but not this singular collapse.

In $d=2$, the sigma energy is scale invariant. The scaling identity supplies no obstruction, but $\pi_2(S^3)=0$ gives no topological soliton sector either. One must not infer nonexistence of every nonconstant stationary harmonic map from these two facts: scale-invariant sigma models can have non-topological harmonic-map saddles, for example using a totally geodesic two-sphere in the target three-sphere. The conclusion is absence of a topologically protected sigma soliton here, with no positive scale-restoring force supplied by the quadratic term alone.

For the [Skyrme model](../../../../../skyrme-model.md), the added commutator term gives the nonnegative static energy

$$
E_4=-\frac1{16}\int\operatorname{Tr}([R_i,R_j][R_i,R_j])\,d^dx.
$$

Anti-Hermiticity of the commutators fixes its sign. The target and boundary condition are unchanged, so the topological classification is unchanged. The [Derrick dimension test for the Skyrme model](../../../../../derrick-dimension-test-for-the-skyrme-model.md) instead becomes

$$
\boxed{E(L)=L^{d-2}E_2+L^{d-4}E_4,\qquad(d-2)E_2+(d-4)E_4=0.}
$$

In $d=3$, the opposite exponents permit a balance:

$$
\boxed{E_2=E_4,\qquad E(L)=LE_2+L^{-1}E_4,\qquad E''(1)=2E_4>0.}
$$

For an arbitrary reference shape with both energies nonzero, its preferred scale is $L_*=(E_4/E_2)^{1/2}$ and its optimized energy is $2\sqrt{E_2E_4}$. Expansion costs quadratic-gradient energy and contraction costs quartic-gradient energy. Integer-degree [Skyrmions](../../../../../skyrmion.md) are therefore topologically possible and evade the pure sigma collapse. This mechanism permits finite-size stable solitons, although existence and stability in all field directions require more than the scaling argument itself.

The other dimensions behave differently. In $d=1$, all spatial commutators vanish identically, so the added term changes nothing and nonconstant static finite-energy fields remain excluded. In $d=2$, stationarity forces $E_4=0$; any configuration with nonzero commutator energy can lower it by spreading. In fact a smooth finite-energy static field of this particular potential-free model must be constant. To prove this [commuting-current obstruction in a two-dimensional Skyrme model](../../../../../commuting-current-obstruction-in-a-two-dimensional-skyrme-model.md), $E_4=0$ forces $[R_1,R_2]=0$ pointwise. The quartic first variation then vanishes, leaving the sigma equation $\partial_iR_i=0$. The right-current [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md) is

$$
\partial_1R_2-\partial_2R_1=[R_1,R_2]=0.
$$

Divergence-free and curl-free currents have componentwise $\Delta R_i=0$. Their components belong to [L2 space](../../../../../l2-space-is-a-hilbert-space.md) by finite $E_2$. An entire square-integrable harmonic function on the plane vanishes: the mean-value formula and Cauchy–Schwarz bound its value by $(\pi R^2)^{-1/2}$ times its full L2 norm, tending to zero as the disk radius $R$ grows. Thus $R_i=0$, and the boundary condition fixes $U=1_2$. This additional argument uses the vanishing commutator; it does not apply to the pure sigma model's general noncommuting currents.

In $d=4$, the virial relation gives $2E_2=0$, hence a constant field and zero $E_4$. In $d>4$ both coefficients are positive and the same conclusion follows. **Only three spatial dimensions allow a nontrivial finite-size balance of these two positive derivative energies.** Higher-dimensional topological classes, where present, do not evade this obstruction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
