<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [strong equivalence principle](../../../../../strong-equivalence-principle.md) asserts universality of free fall, including gravitational self-energy, and local independence of nongravitational and gravitational experiments from a freely falling laboratory's location and velocity. In a sufficiently small [local inertial frame](../../../../../local-inertial-frame.md), uniform gravitational acceleration is removed and local physics takes its special-relativistic form. The [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) remains measurable through tidal effects; a finite laboratory is not made exactly flat. Freely falling test bodies follow [geodesics](../../../../../geodesic.md), clocks measure [proper time](../../../../../proper-time.md), and minimally coupled light follows [null geodesics](../../../../../null-geodesic.md) in [geometrical optics](../../../../../geometrical-optics.md). Local nongravitational laws retain their special-relativistic form even when different laboratories observe [gravitational redshift](../../../../../gravitational-redshift.md).

The [comma-to-semicolon prescription](../../../../../comma-to-semicolon-prescription.md) replaces flat partial derivatives by the [Levi-Civita connection](../../../../../levi-civita-connection.md), and the [Minkowski metric](../../../../../minkowski-metric.md) by the curved [metric tensor](../../../../../metric-tensor.md). It implements this local correspondence for minimally coupled matter. However, an identity obtained by commuting partial derivatives need not survive unchanged when they become [covariant derivatives](../../../../../covariant-derivative.md).

Raising the indices of the field-strength definition in flat spacetime gives $F^{ab}=\partial^aA^b-\partial^bA^a$. Substitution into the sourced [Maxwell equations](../../../../../maxwell-equations.md) yields

$$
\partial_b\partial^aA^b-\partial_b\partial^bA^a=-\mu_0J^a,
$$

so the first potential equation is

$$
\boxed{\Box A^a-\partial_b\partial^aA^b=\mu_0J^a.}
$$

Partial derivatives commute, giving the second form

$$
\boxed{\Box A^a-\partial^a(\partial_bA^b)=\mu_0J^a.}
$$

No [Lorenz gauge](../../../../../lorenz-gauge-condition.md) assumption was used.

Apply the [comma-to-semicolon prescription](../../../../../comma-to-semicolon-prescription.md) before commuting derivatives. The two candidate left-hand sides become

$$
\mathcal P_1^a=\nabla_b\nabla^bA^a-\nabla_b\nabla^aA^b,\qquad
\mathcal P_2^a=\nabla_b\nabla^bA^a-\nabla^a(\nabla_bA^b).
$$

Use the cover curvature $C$ from Question 1, with $C_{ab}=C^c{}_{acb}$. The vector commutator is $[\nabla_c,\nabla_d]A^a=-C^a{}_{bcd}A^b$. Hence

$$
\nabla_b\nabla^aA^b-\nabla^a\nabla_bA^b=-C^a{}_bA^b,
\qquad
\boxed{\mathcal P_1^a=\mathcal P_2^a+C^a{}_bA^b.}
$$

This is the [derivative-order ambiguity in covariant Maxwell potential equations](../../../../../derivative-order-ambiguity-in-covariant-maxwell-potential-equations.md). At a point in [Riemann normal coordinates](../../../../../normal-coordinates.md), the connection itself vanishes but its derivatives need not; the [strong equivalence principle](../../../../../strong-equivalence-principle.md) does not dispose of this curvature term by a coordinate choice.

Covariantizing the antisymmetric field strength and its [Maxwell equations](../../../../../maxwell-equations.md) directly gives $\mathcal P_1^a=\mu_0J^a$, or

$$
\boxed{\Box A^a-\nabla^a(\nabla_bA^b)+C^a{}_bA^b=\mu_0J^a.}
$$

This formulation has [gauge invariance](../../../../../gauge-invariance.md) under $A_a\mapsto A_a+\nabla_a\chi$, since $F_{ab}$ is unchanged. In contrast, the uncorrected $\mathcal P_2$ acquires $-C^a{}_b\nabla^b\chi$ under that transformation. Thus preserving the original electromagnetic [gauge symmetry](../../../../../gauge-invariance.md) singles out the directly covariantized [Maxwell equations](../../../../../maxwell-equations.md), rather than treating the two potential equations as interchangeable in matter. The [Equivalence principle](../../../../../equivalence-principle.md) alone is not a unique recipe for every possible higher-derivative or curvature coupling.

In a Ricci-flat [vacuum spacetime](../../../../../vacuum-spacetime.md), $C_{ab}=0$, so $\mathcal P_1=\mathcal P_2$ and this particular ambiguity disappears even though the full [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) may be nonzero. This uses vacuum with zero [cosmological constant](../../../../../cosmological-constant.md); an Einstein vacuum with nonzero cosmological constant is not Ricci flat.

For the terrestrial estimate, the relevant effect is Ricci curvature inside matter, not merely the tidal field outside the Earth. If a typical material density is $\rho\sim5\,\mathrm{g\,cm^{-3}}$, the [Einstein field equations](../../../../../einstein-field-equations.md) give a characteristic scale

$$
|C^a{}_b|\sim8\pi G\rho\sim9\times10^{-27}\,\mathrm{cm^{-2}}.
$$

For a field varying over scale $L$, the derivative terms are $O(A/L^2)$ whereas the disputed term is $O(CA)$. Their relative size is $O(CL^2)$: about $10^{-22}$ for a metre-scale experiment. Even substituting the Earth's radius gives only

$$
CL^2\big|_{L=R}\sim(9\times10^{-27})(6\times10^8)^2\sim3\times10^{-9}.
$$

A curvature length comparable to $C^{-1/2}\sim10^{13}\,\mathrm{cm}$ would be needed for an order-one effect. **In principle non-vacuum measurements could distinguish different curvature couplings, but an ordinary terrestrial laboratory has an exceedingly small signal**, overwhelmed by its ordinary electromagnetic response to matter. This is a practical scale estimate, not a theorem that an arbitrarily precise experiment is impossible.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
