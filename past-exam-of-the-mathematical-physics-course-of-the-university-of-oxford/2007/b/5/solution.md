<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use [metric signature](../../../../metric-signature.md) $(+---)$ and the [curvature](../../../../curvature.md) sign fixed by the stated [Newtonian limit](../../../../newtonian-limit.md). In flat spacetime the source-free [Maxwell equations](../../../../maxwell-equations-split.md) are $\partial_aF^{ab}=0$ and $\partial_{[a}F_{bc]}=0$. The [stress-energy tensor](../../../../stress-energy-tensor-split.md) in mixed form is $T^a{}_b=F^{ac}F_{cb}+\delta^a_bF_{cd}F^{cd}/4$. Its divergence is

$$
\partial_aT^a{}_b=(\partial_aF^{ac})F_{cb}+F^{ac}\partial_aF_{cb}+\frac14\partial_b(F_{cd}F^{cd}).
$$

Contracting the cyclic Maxwell equation with $F^{ac}$ gives $F^{ac}\partial_aF_{cb}=-\partial_b(F_{cd}F^{cd})/4$. The first term also vanishes, proving $\boxed{\partial_aT^{ab}=0}$. The component $b=0$ expresses local electromagnetic [energy conservation](../../../../conservation-of-energy.md), and the spatial components express [momentum conservation](../../../../momentum-conservation.md). Integrating converts them into the usual energy and momentum flux balances.

In curved spacetime the [tensor](../../../../tensor.md) equations are

$$
\boxed{\nabla_aF^{ab}=0,\qquad\nabla_{[a}F_{bc]}=0.}
$$

They agree with the flat equations in coordinates of a [local inertial frame](../../../../local-inertial-frame.md) at a point, where the connection vanishes, and covariance then extends them to arbitrary coordinates. [Antisymmetry](../../../../antisymmetry.md) makes the homogeneous equation equivalent to $dF=0$. [Metric compatibility](../../../../metric-compatibility.md) permits the same contraction proof, now giving $\boxed{\nabla_aT^{ab}=0}$. In general,

$$
\partial_aT^{ab}=-\Gamma^a{}_{ac}T^{cb}-\Gamma^b{}_{ac}T^{ac},
$$

which need not vanish. Covariant local balance remains valid; ordinary coordinate components do not provide a universal conserved global energy-momentum vector in a curved geometry. Additional spacetime symmetries can furnish conserved currents. A locally inertial frame removes the connection at a point, not the [curvature](../../../../curvature.md) or the global obstruction.

The alternating array with fixed component $\epsilon_{0123}=1$ is appropriate in oriented inertial special-relativistic coordinates, whose proper [Lorentz transformations](../../../../lorentz-transformation.md) have determinant one. It is not itself a covariant [tensor](../../../../tensor.md) under general coordinate changes. For an oriented [Lorentzian metric](../../../../lorentzian-metric.md), replace it by the metric [metric volume tensor](../../../../metric-volume-tensor.md) $\varepsilon_{abcd}=\sqrt{-\det g}\,[abcd]$. The genuine dual is

$$
\boxed{(*F)_{ab}=\tfrac12\varepsilon_{abcd}F^{cd}.}
$$

This is the [Hodge star](../../../../hodge-star-operator.md); the determinant factor, [orientation](../../../../orientation-of-a-simplex.md) and raising conventions are essential. Even in flat spacetime arbitrary curvilinear coordinates require the [metric volume tensor](../../../../metric-volume-tensor.md), so the distinction is about coordinate covariance rather than [curvature](../../../../curvature.md) alone.

The isolated equation for $R_{00}$ singles out a coordinate component and cannot be a generally covariant law. Replacing it by a proportionality $R_{ab}\propto T_{ab}$ still fails: the [contracted Bianchi identity](../../../../contracted-bianchi-identity.md) gives $\nabla^aR_{ab}=\nabla_bR/2$, whereas stress-[energy conservation](../../../../conservation-of-energy.md) requires $\nabla^aT_{ab}=0$. Such a law would force $R$ constant and hence impose an unphysical restriction on a varying [relativistic dust](../../../../relativistic-dust.md) density. Missing units or a coupling constant in the proposed proportionality would not repair this structural problem.

The [Einstein tensor](../../../../einstein-tensor.md) $G_{ab}=R_{ab}-Rg_{ab}/2$ is divergence-free. Therefore

$$
\boxed{G_{ab}=-8\pi G T_{ab}}
$$

is consistent with covariant stress-[energy conservation](../../../../conservation-of-energy.md) in the source's [curvature](../../../../curvature.md) convention. Its trace gives $R=8\pi GT$ and hence $R_{ab}=-8\pi G(T_{ab}-Tg_{ab}/2)$. For slowly moving [relativistic dust](../../../../relativistic-dust.md) with $V^aV_a=1$, $T_{00}\simeq\rho$, $T\simeq\rho$, $g_{00}\simeq1$, so $R_{00}\simeq-4\pi G\rho$, exactly matching $-\Delta\phi$ and Poisson's equation.

Finally, electromagnetic stress-energy is trace-free: $T^a{}_a=F^{ac}F_{ca}+F_{cd}F^{cd}=0$ by [antisymmetry](../../../../antisymmetry.md). The traced field equation then gives $\boxed{R=0}$ for a purely electromagnetic source. This does not say $R_{ab}=0$ or that spacetime is flat; its trace-free [Ricci curvature](../../../../ricci-curvature.md) can still be nonzero.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematical physics course of the University of Oxford](../../../split.md)
5. [Mathematical physics course of the University of Oxford](../../../../mathematical-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
