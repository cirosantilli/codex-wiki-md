<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [normal form](../../../../../../normal-form-dynamical-systems.md) is invariant under $z\mapsto e^{i\varphi}z$. This continuous [rotational symmetry](../../../../../../rotational-symmetry.md) makes the axis invariant and reduces the nontrivial geometry to two amplitude variables. The axis connection from $E_+$ to $E_-$ persists without parameter tuning, while rotating the outer connection produces a family of connections from $E_-$ back to $E_+$. A two-dimensional autonomous amplitude flow cannot by itself produce the proposed saddle-focus return chaos: symmetry reduction hides the phase-dependent reinjection needed for that mechanism.

Generic higher-order terms need not retain this exact [rotational symmetry](../../../../../../rotational-symmetry.md). A [normal form](../../../../../../normal-form-dynamical-systems.md) can preserve it to a finite truncation order while the full equations have small symmetry-breaking remainders. These unfold the special connection geometry into phase-dependent returns; nearby parameter curves can contain [homoclinic orbits](../../../../../../homoclinic-orbit.md) to a [saddle-focus](../../../../../../saddle-focus-equilibrium.md), and the [Shilnikov bifurcation](../../../../../../shilnikov-bifurcation.md) mechanism becomes available. Their exact placement depends on the omitted terms and is not fixed by the displayed truncation alone.

For example, at the perturbed positive-axis saddle, the real unstable [eigenvalue](../../../../../../eigenvalue.md) is $\lambda_u=2a$ and the stable complex pair has real part $\mu_1-2a+a^2$. Near the calculated connection curve $\mu_1=-a^2/4+o(a^2)$, the contracting ratio is

$$
\delta=-\frac{\operatorname{Re}\lambda_s}{\lambda_u}
=1-\frac{3a}{8}+o(a)<1.
$$

This is the positive-saddle-value regime, explaining why the relevant saddle-focus return can be expanding.

In the [Shilnikov return map](../../../../../../shilnikov-return-map.md), take a positive return coordinate $y$ and $0<\delta<1$, with nondegenerate $A\ne0,B\ne0$. At the connection parameter $\mu=0$, the [fixed point](../../../../../../fixed-point.md) condition is

$$
\cos(B\log y+\Phi)=y^{1-\delta}/A.
$$

The right side tends to zero, whereas the phase passes through infinitely many oscillations as $y\downarrow0$. Hence there are infinitely many positive [fixed points](../../../../../../fixed-point.md) accumulating at zero, with logarithmically spaced amplitudes. For these points,

$$
f'(y)=Ay^{\delta-1}\{\delta\cos(B\log y+\Phi)-B\sin(B\log y+\Phi)\},
$$

whose magnitude tends to infinity along the accumulating fixed-point sequence. They represent long-period saddle [periodic orbits](../../../../../../periodic-orbit.md) of the full return, with period growing like $\lambda_u^{-1}\log(1/y)$, rather than infinitely many stable cycles.

Successive turning branches of this oscillatory return can stretch and fold across suitable intervals. The full saddle-focus [Poincaré return map](../../../../../../poincare-map.md) then admits invariant [Smale horseshoes](../../../../../../smale-horseshoe.md) and chaotic itineraries near a generic [homoclinic orbit](../../../../../../homoclinic-orbit.md) at a [Shilnikov bifurcation](../../../../../../shilnikov-bifurcation.md). Varying $\mu$ unfolds accumulating saddle-node and period-doubling events. Whether any resulting invariant set attracts trajectories depends on the other return direction and the omitted terms; the leading scalar map alone does not prove a chaotic attractor for every perturbation. Its domain also excludes negative iterates, which leave the chosen return branch. The degeneracies $A=0$ or $B=0$ would remove the oscillatory mechanism, so the conclusion uses generic, genuinely saddle-focus reinjection.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
