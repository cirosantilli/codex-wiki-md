<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Because $\langle B\rangle=0$, a periodic primitive $H$ exists. Fix its additive constant by $\langle H\rangle=0$. Integrating the conserved-field equation once in space gives $H_T=\sigma(H_X+\delta A^2)_X$: the possible integration constant vanishes on taking the spatial mean. Treat the spatial average as the inner product defining [functional derivatives](../../../../../../functional-derivative.md). [Integration by parts](../../../../../../integration-by-parts.md), with no boundary terms under [periodic boundary conditions](../../../../../../periodic-boundary-conditions.md), gives

$$
\frac{\delta V}{\delta A}=\mu A+\alpha A^2-A^3+A_{XX}-AH_X=A_T,\qquad
\frac{\delta V}{\delta H}=\frac12(A^2)_X+\frac{H_{XX}}{2\delta}=\frac{H_T}{2\delta\sigma}.
$$

Thus the [conserved-field real amplitude equation](../../../../../../conserved-field-real-amplitude-equation.md) is a [gradient flow](../../../../../../gradient-flow.md) ascending $V$, or descending $-V$, with positive diagonal mobilities. Along a classical solution,

$$
\boxed{\frac{dV}{dT}=\left\langle A_T^2+\frac{H_T^2}{2\delta\sigma}\right\rangle\geq0.}
$$

For the mixed term put $P=\langle A^4\rangle^{1/2}$ and $Q=\langle H_X^2\rangle^{1/2}$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and a completed square give

$$
\left\langle-\frac12A^2H_X-\frac{H_X^2}{4\delta}\right\rangle
\leq\frac{PQ}{2}-\frac{Q^2}{4\delta}
=\frac{\delta P^2}{4}-\frac{(Q-\delta P)^2}{4\delta}
\leq\frac\delta4\langle A^4\rangle.
$$

Consequently, for $\beta=1-\delta>0$,

$$
V\leq\left\langle\frac\mu2A^2+\frac\alpha3A^3-\frac\beta4A^4-\frac12A_X^2\right\rangle
\leq\max_{a\in\mathbb R}\left(\frac\mu2a^2+\frac\alpha3a^3-\frac\beta4a^4\right)<\infty.
$$

The negative leading quartic coefficient proves the upper bound. The stronger pointwise square completion

$$
V=\left\langle\frac\mu2A^2+\frac\alpha3A^3-\frac\beta4A^4-\frac12A_X^2-\frac{(H_X+\delta A^2)^2}{4\delta}\right\rangle
$$

is also useful: a superlevel set $V\geq V(0)$ bounds the amplitude in $L^4$, its spatial [derivative](../../../../../../derivative.md) in $L^2$, and $B=H_X$ in $L^2$, because a quartic [polynomial](../../../../../../polynomial-split.md) with negative leading coefficient dominates its lower-order terms.

**The dynamics dissipates toward the steady-state set rather than sustaining nonconstant periodic motion.** Indeed $V$ increases to a finite limit, and the time integral of $\langle A_T^2+H_T^2/(2\delta\sigma)\rangle$ is finite. For global regular trajectories with the usual parabolic precompactness, every limit point is stationary, by the [LaSalle invariance principle](../../../../../../lasalle-s-invariance-principle.md). A nonconstant periodic or recurrent orbit would force a strictly increasing $V$ to return to its original value and is impossible. Boundedness of a monotone functional alone does not prove convergence to one particular [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md); isolation of the limiting [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) or an additional convergence theorem supplies that stronger claim.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
