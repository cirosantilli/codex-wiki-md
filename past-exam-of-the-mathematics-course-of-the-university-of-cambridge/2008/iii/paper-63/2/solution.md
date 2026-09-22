<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $z$ positive outward and define the separation as upper minus lower position. The [Newtonian potential of a point mass](../../../../../newtonian-potential-of-a-point-mass.md) gives the acceleration $a(z)=-\partial_z\phi=-GM/z^2$. Expanding its difference across a separation $\zeta\ll z$ gives the [tidal force](../../../../../tidal-force.md) equation

$$
\ddot\zeta=a(z+\zeta)-a(z)=a'(z)\zeta+O(\zeta^2/z^2)
\simeq\boxed{\frac{2GM}{z^3}\zeta}.
$$

The upper particle falls slightly less rapidly, so the separation increases. If the upper particle carries the [electric charge](../../../../../electric-charge.md) and the [electric field](../../../../../electric-field.md) points outward, the extra relative acceleration is $qE/m$. Reversing the field or placing the charge on the lower particle changes its sign. Write this signed acceleration as $a_e$ and put $k=2GM/z^3$. With initial relative velocity zero and nearly constant $k$ and $a_e$, the [ordinary differential equation](../../../../../ordinary-differential-equation.md) has solution

$$
\zeta(t)=\zeta_0\cosh(\sqrt{k}\,t)
+\frac{a_e}{k}\bigl[\cosh(\sqrt{k}\,t)-1\bigr].
$$

For $kt^2\ll1$, the leading changes due to the [tidal force](../../../../../tidal-force.md) and [electric field](../../../../../electric-field.md) are respectively

$$
\boxed{\Delta\zeta_g\simeq\frac{GM}{z^3}\zeta_0t^2,
\qquad \Delta\zeta_e\simeq\frac{qE}{2m}t^2}
$$

with the stated sign convention. Thus, for a nonzero fixed electric acceleration,

$$
\frac{|\Delta\zeta_g|}{|\Delta\zeta_e|}
\simeq\frac{2mGM|\zeta_0|}{|qE|z^3}
=\frac{2mg}{|qE|}\frac{|\zeta_0|}{z},
\qquad g=\frac{GM}{z^2}.
$$

A laboratory of size $L$ has $|\zeta_0|\leq L$, so this ratio tends to zero as $L\to0$. This is [local tidal acceleration scaling](../../../../../local-tidal-acceleration-scaling.md): gravitational relative acceleration is proportional to separation, whereas the electric difference persists even at coincident positions.

The duration also matters. At fixed time, $\Delta\zeta_g\to0$ in absolute size, but $\Delta\zeta_g/\zeta_0\simeq(GM/z^3)t^2$ need not tend to zero. To keep the electrically displaced particles in the shrinking laboratory, take $|a_e|t^2\lesssim L$; then $|\Delta\zeta_g|/L\lesssim GM L/(z^3|a_e|)\to0$. Alternatively a stationary terrestrial laboratory has a free-fall time of order $\sqrt{L/g}$, giving $|\Delta\zeta_g|/|\zeta_0|=O(L/z)$. Both make precise the small spacetime-region limit. An extended, long-running experiment can still measure arbitrarily small [tidal forces](../../../../../tidal-force.md).

The [weak equivalence principle](../../../../../weak-equivalence-principle.md) says that freely falling [test particles](../../../../../test-particle.md) with the same initial data have composition-independent motion. In particular, a freely falling frame removes the common gravitational acceleration of both particles. The electric accelerations depend on charge and cannot be removed for charged and uncharged particles simultaneously by the same change of frame.

The [Einstein equivalence principle](../../../../../einstein-equivalence-principle.md) extends the freely falling laboratory statement to all local nongravitational experiments: their outcomes obey [special relativity](../../../../../special-relativity-split.md), with local Lorentz invariance and local position invariance. The [strong equivalence principle](../../../../../strong-equivalence-principle.md) also includes local gravitational experiments and bodies with significant gravitational binding energy. It asserts universality of their free fall and independence of local experimental outcomes from the laboratory's location and velocity. The two-particle experiment illustrates the local distinction between gravity and a nongravitational force; by itself it does not establish this stronger claim about self-gravitating bodies.

In a metric theory, the common freely falling trajectories are [timelike geodesics](../../../../../timelike-geodesic.md) of a [Lorentzian metric](../../../../../lorentzian-metric.md). [Normal coordinates](../../../../../normal-coordinates.md) make $g_{ab}=\eta_{ab}$ and the [Christoffel symbols](../../../../../christoffel-symbol.md) zero at one point. [Fermi normal coordinates](../../../../../fermi-coordinates.md) do the same along a reference [timelike geodesic](../../../../../timelike-geodesic.md). The residual effects are controlled by the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) through [geodesic deviation](../../../../../geodesic-deviation.md), and enter the local metric at quadratic order in distance. Curvature is a physical tidal field, so no coordinate choice removes it over a finite region.

A relativistic theory should consequently couple matter universally to the [metric tensor](../../../../../metric-tensor.md), recover nongravitational laws in local inertial frames and recover the Newtonian limit. [General relativity](../../../../../general-relativity-split.md) implements this with the [Einstein field equations](../../../../../einstein-field-equations.md); the [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) is consistent with [stress-energy conservation](../../../../../stress-energy-conservation.md). The [Equivalence principle](../../../../../equivalence-principle.md) motivates this geometric description but does not alone uniquely determine the field equations. Extra gravitational fields may satisfy the [Einstein equivalence principle](../../../../../einstein-equivalence-principle.md) for ordinary matter while failing the [strong equivalence principle](../../../../../strong-equivalence-principle.md) because local gravitational measurements or self-gravitating trajectories depend on those fields.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
