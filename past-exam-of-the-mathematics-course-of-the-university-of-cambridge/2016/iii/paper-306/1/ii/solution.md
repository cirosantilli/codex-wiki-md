<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the [open-string endpoint momentum flux](../../../../../../open-string-endpoint-momentum-flux.md) along the [open string](../../../../../../open-string.md) by $J_m=eT^2X'_m+uP_m$. Variation of the [Nambu-Goto phase-space action](../../../../../../nambu-goto-phase-space-action.md) gives

$$
\boxed{\dot X^m=eP^m+uX'^m,\qquad\dot P_m=\partial_\sigma J_m,}
$$



$$
\boxed{P^2+T^2X'^2=0,\qquad X'\cdot P=0.}
$$

The two last equations are the [Virasoro constraints](../../../../../../virasoro-constraint.md). Integration of the [momentum](../../../../../../momentum.md) equation gives

$$
\boxed{\dot{\mathcal P}_m=J_m(t,\pi)-J_m(t,0).}
$$

Thus the necessary and sufficient condition for total [momentum conservation](../../../../../../momentum-conservation.md) is equality of the two endpoint fluxes, component by component. Vanishing of both fluxes is a sufficient local boundary condition.

The spatial boundary term in the action variation is $-\int dt[J_m\delta X^m]_0^\pi$. For free ends the endpoint variations are arbitrary, so

$$
\boxed{J_m|_{0,\pi}=0\quad\Longrightarrow\quad\dot{\mathcal P}_m=0.}
$$

In a gauge with $u=0$ and nonzero $e$ this reduces to the usual [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) $X'^m=0$. The conclusion is conservation of total [momentum](../../../../../../momentum.md), not that total [momentum](../../../../../../momentum.md) must vanish. The PDF contains the derivative in this conclusion; the TeX transcription drops it.

For endpoints confined to $x^1=0$, the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) fixes $\delta X^1=0$. It therefore imposes no requirement that $J_1$ vanish. Preserving the fixed position requires $\dot X^1=eP^1+uX'^1=0$ at each endpoint, but that is a different condition. For example, in $u=0$ gauge the endpoint [momentum](../../../../../../momentum.md) $P^1$ is zero while $eT^2X'^1$ can be nonzero. Consequently **$\mathcal P_1$ is generally not conserved**: the normal endpoint forces transfer [momentum](../../../../../../momentum.md) to the hyperplane. A dynamical [D-brane](../../../../../../d-brane.md) recoils and carries the missing [momentum](../../../../../../momentum.md). If the hyperplane is idealized as fixed, its external support absorbs the [momentum](../../../../../../momentum.md). The combined string-and-support system conserves [momentum](../../../../../../momentum.md); freely varying directions tangent to the hyperplane retain their vanishing-flux condition.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
