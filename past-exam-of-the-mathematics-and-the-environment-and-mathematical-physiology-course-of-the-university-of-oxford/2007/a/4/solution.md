<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Basal sliding](../../../../basal-sliding.md) allows ice to pass over bed obstacles by enhanced deformation and [regelation](../../../../regelation.md): pressure-induced melting on the upstream side and refreezing downstream transfer ice around small obstacles. [Cavitation](../../../../cavitation.md) opens water-filled gaps on the downstream side. Their size and the remaining ice-bed contact depend on [effective pressure in subglacial drainage](../../../../effective-pressure-in-subglacial-drainage.md) $N=p_{\rm ice}-p_{\rm water}$ as well as basal [shear stress](../../../../shear-stress.md) $\tau$. At fixed $\tau$, reducing $N$ generally enlarges cavities and reduces resistance, giving a sliding law $u(\tau,N)$ with $u_N<0$ in this regime.

A [linked cavity drainage system](../../../../linked-cavity-drainage-system.md) connects these cavities through passages along the bed. Under the prescribed decreasing relation $N(Q)$, the [chain rule](../../../../chain-rule.md) gives $\boxed{u_Q=u_NN'(Q)>0}$. This conclusion uses that hydraulic relation; it need not apply to a different drainage regime.

With $t=\varepsilon\tau$, the ice continuity equation becomes $H_\tau+\varepsilon(uH)_x=\varepsilon s'(x)$. For bounded spatial gradients over $\tau=O(1)$, $H$ is independent of the fast seasonal time to leading order. Meanwhile $S'(Q)=\varepsilon\kappa$ gives $S_t=\kappa Q_\tau$, so

$$
\boxed{\kappa Q_\tau+Q_x=M(\tau).}
$$

Let $J(\tau)=\int_0^\tau M(r)\,dr$. Direct differentiation proves that

$$
\boxed{Q(x,\tau)=\frac{J(\tau)-J(\tau-\kappa x)}\kappa}
$$

satisfies the equation and $Q(0,\tau)=0$. This is the boundary-generated solution, or a periodic-forcing solution with the forcing continued into its past. An independently prescribed initial profile would also need matching in the region whose [characteristic curves](../../../../characteristic-curve.md) have not yet reached the upstream boundary.

If $M>0$, $J$ is invertible and rearranging gives $x=[\tau-J^{-1}(J(\tau)-\kappa Q)]/\kappa$. For $M=1-\delta\cos\tau$ with $|\delta|<1$,

$$
\boxed{J(\tau)=\tau-\delta\sin\tau,\qquad J^{-1}(\theta)=\theta+\delta\sin\theta+O(\delta^2).}
$$

Substitution, followed by the sine-difference identity, gives

$$
\boxed{x=Q+\frac{2\delta}{\kappa}\sin\frac{\kappa Q}{2}\cos\left(\tau-\frac{\kappa Q}{2}\right)+O(\delta^2).}
$$

For fixed $Q$ and nonzero first-order amplitude, the extrema occur at $\tau=\kappa Q/2+n\pi+O(\delta)$. Since $x=Q+O(\delta)$, the [seasonal phase lag in linked cavity drainage](../../../../seasonal-phase-lag-in-linked-cavity-drainage.md) gives the stated phase relation $\boxed{\tau\approx\kappa x/2\pmod\pi}$. Maxima and minima alternate; when $\sin(\kappa Q/2)=0$, the first-order approximation is flat and does not locate individual extrema.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
