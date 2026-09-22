<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

[Noether's theorem](../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md) associates a continuous one-parameter differentiable symmetry of the [action](../../../../action.md) with an on-shell conserved current. If a first-derivative [Lagrangian density](../../../../lagrangian-density.md) varies by $\delta\mathcal L=\partial_\mu B^\mu$, the current is $J^\mu=\mathcal L_{\partial_\mu\phi}\delta\phi-B^\mu$. The [integral](../../../../integral-split.md) of $J^0$ is conserved when the spatial boundary flux vanishes. This connects symmetries to [conservation laws](../../../../conservation-law.md); time translation, spatial translation and internal [phase](../../../../phase-waves.md) symmetry furnish familiar examples.

For the strict fixed-coordinate invariance in the question, $B^\mu=0$. In one space dimension, [integration by parts](../../../../integration-by-parts.md) at the [density](../../../../density.md) level gives

$$
\delta\mathcal L=
\left[\mathcal L_\phi-\partial_t\mathcal L_{\dot\phi}-\partial_x\mathcal L_{\phi'}\right]\delta\phi
+\partial_t(\mathcal L_{\dot\phi}\delta\phi)
+\partial_x(\mathcal L_{\phi'}\delta\phi).
$$

The bracket vanishes by the field equation. Thus $\delta\mathcal L=0$ yields

$$
\boxed{\partial_t\rho+\partial_xJ_x=0,\qquad
\rho=\mathcal L_{\dot\phi}\delta\phi,\qquad
J_x=\mathcal L_{\phi'}\delta\phi.}
$$

In four [spacetime](../../../../spacetime.md) dimensions the same identity gives $\partial_\mu J^\mu=0$ with $J^\mu=\mathcal L_{\partial_\mu\phi}\delta\phi$. In particular, for the usual scalar kinetic term the spatial current has the minus sign inherited from $\partial^i=-\partial_i$.

For the quartic [density](../../../../density.md) in $n$ dimensions,

$$
\mathcal L_\phi=-4\lambda\phi^3,\qquad
\mathcal L_{\partial_\mu\phi}=\partial^\mu\phi,
\qquad\boxed{\Box\phi+4\lambda\phi^3=0.}
$$

To evaluate the displayed dilation current, abbreviate $S=(\partial_\mu\phi)(\partial^\mu\phi)$ and $D=x^\nu\partial_\nu$. Product differentiation gives

$$
\begin{aligned}
\partial_\mu J^\mu
&=2S+(D\partial_\mu\phi)\partial^\mu\phi
+(\phi+D\phi)\Box\phi-n\mathcal L-D\mathcal L\\
&=2S-4\lambda\phi^4-n\mathcal L
+(\phi+D\phi)(\Box\phi+4\lambda\phi^3)\\
&=(4-n)\mathcal L+(\phi+D\phi)(\Box\phi+4\lambda\phi^3).
\end{aligned}
$$

Here $D(S/2)=(D\partial_\mu\phi)\partial^\mu\phi$ makes the differentiated kinetic terms cancel, and $D(\lambda\phi^4)=4\lambda\phi^3D\phi$. [On shell](../../../../on-shell.md), the [on-shell divergence of a quartic scalar dilation current](../../../../on-shell-divergence-of-a-quartic-scalar-dilation-current.md) reduces to

$$
\boxed{\partial_\mu J^\mu=(4-n)\mathcal L.}
$$

Hence this current is conserved for generic solutions in **four [spacetime](../../../../spacetime.md) dimensions**. Special field configurations with vanishing [density](../../../../density.md) do not alter the generic dimensional statement.

The subtraction $-x^\mu\mathcal L$ has a symmetry explanation: for $\delta\phi=\phi+D\phi$, direct variation gives $\delta\mathcal L=D\mathcal L+4\mathcal L=\partial_\mu(x^\mu\mathcal L)+(4-n)\mathcal L$. At $n=4$ the [action](../../../../action.md) is invariant up to a [boundary term](../../../../boundary-term.md), so $B^\mu=x^\mu\mathcal L$. Strict invariance of the [density](../../../../density.md) is not required. This is a classical result; no claim about quantum [scale invariance](../../../../scale-invariance.md) is needed.

## ↑ Ancestors (14)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
