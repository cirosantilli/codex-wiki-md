<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [Lie algebra homomorphism](../../../../../../lie-algebra-homomorphism.md) $\theta:\mathfrak g_1\to\mathfrak g_2$ always defines a local [group homomorphism](../../../../../../group-homomorphism.md) near the identities by the exponential charts:

$$
\phi(\exp X)=\exp(\theta X)
$$

for sufficiently small $X$. Preservation of the BCH multiplication law makes this a local [homomorphism](../../../../../../homomorphism.md). The issue is extending it consistently around all paths and periods in the source.

Suppose first that $G_1$ is connected and [simply connected](../../../../../../simply-connected-space.md). For a piecewise smooth path $\gamma:[0,1]\to G_1$ from $e_1$ to $g$, let

$$
A(t)=d_{\gamma(t)}L_{\gamma(t)^{-1}}\,\dot\gamma(t)
$$

be its left logarithmic velocity. Solve in $G_2$ the differential equation

$$
\dot\eta(t)=d_{e_2}L_{\eta(t)}\,\theta(A(t)),\qquad\eta(0)=e_2.
$$

The equation exists throughout the finite path interval: bounded smooth body velocity gives a uniform local existence interval at the identity, and [left translation](../../../../../../left-and-right-translation-on-a-lie-group.md) repeatedly continues the solution. Define the proposed map by the endpoint $\Phi(g)=\eta(1)$.

Bracket preservation makes this endpoint invariant under fixed-endpoint [homotopy](../../../../../../homotopy.md). To see the mechanism, for a two-parameter path write $A=\gamma^{-1}\partial_t\gamma$ and $B=\gamma^{-1}\partial_s\gamma$, using the [Maurer-Cartan form](../../../../../../maurer-cartan-form.md) rather than literal multiplication for nonmatrix [groups](../../../../../../group-split.md). The [Maurer-Cartan equation](../../../../../../maurer-cartan-equation.md) gives

$$
\partial_sA-\partial_tB=[A,B].
$$

After applying $\theta$, the same identity holds for $a=\theta A$ and $b=\theta B$. If $c=\eta^{-1}\partial_s\eta$, the transport equation implies

$$
\partial_tc=\partial_sa-[a,c],\qquad
\partial_tb=\partial_sa-[a,b].
$$

Both have zero initial value because the path starts at a fixed identity. Uniqueness gives $c=b$. At the fixed endpoint, $B(s,1)=0$, hence $\partial_s\eta(s,1)=0$. The endpoint is therefore unchanged by the [homotopy](../../../../../../homotopy.md). Simple connectedness then makes it independent of the chosen path.

For paths to $g$ and $h$, concatenate the first with the left translate by $g$ of the second. Its transported endpoint is $\Phi(g)\Phi(h)$, because left logarithmic velocity is unchanged by [left translation](../../../../../../left-and-right-translation-on-a-lie-group.md). It follows that $\Phi(gh)=\Phi(g)\Phi(h)$. Near the identity, choose $\gamma(t)=\exp(tX)$; transport yields $\Phi(\exp X)=\exp(\theta X)$. Thus $\Phi$ is smooth near the identity and, by translation, everywhere, and its differential is $\theta$. The uniqueness argument from the root solution gives

$$
\boxed{\text{A connected simply connected source admits a unique global }\Phi\text{ with }d_e\Phi=\theta.}
$$

This is [integration of a Lie algebra homomorphism](../../../../../../integration-of-a-lie-algebra-homomorphism.md).

For a connected source that is not [simply connected](../../../../../../simply-connected-space.md), first integrate $\theta$ on its [universal cover](../../../../../../universal-cover.md) $p:\widetilde G_1\to G_1$. The resulting map $\widetilde\Phi:\widetilde G_1\to G_2$ descends exactly when

$$
\boxed{\widetilde\Phi(\ker p)=\{e_2\}.}
$$

Indeed two lifts of one element differ by a kernel element, so this condition is both necessary and sufficient for their images to agree. It is the [period obstruction to integration of a Lie algebra homomorphism](../../../../../../period-obstruction-to-integration-of-a-lie-algebra-homomorphism.md). For $G_1=G_2=S^1$, identify the [Lie algebras](../../../../../../lie-algebra-split.md) with $\mathbb R$ and take $\theta(t)=ct$. The integrated map on the cover is $t\mapsto e^{ict}$, which respects the source period $2\pi$ precisely when $c\in\mathbb Z$. Therefore half-scaling is a valid [Lie algebra homomorphism](../../../../../../lie-algebra-homomorphism.md) but does not integrate to a circle [homomorphism](../../../../../../homomorphism.md). If both [groups](../../../../../../group-split.md) are written as [simply connected](../../../../../../simply-connected-space.md) covers modulo central [subgroups](../../../../../../subgroup.md), the equivalent descent condition is that the integrated cover map send $\Gamma_1$ into $\Gamma_2$.

For disconnected $G_1$, first solve this problem on $G_1^\circ$, obtaining $\phi_0$. One must then assign images $a_\gamma$ to representatives $s_\gamma$ of the component [group](../../../../../../group-split.md). These assignments must satisfy the conjugation and multiplication relations. Explicitly, with $s_e=e$ and $s_\gamma s_\delta=s_{\gamma\delta}c_{\gamma,\delta}$ for $c_{\gamma,\delta}\in G_1^\circ$, the conditions are

$$
a_\gamma\phi_0(h)a_\gamma^{-1}
=\phi_0(s_\gamma h s_\gamma^{-1}),\qquad
a_\gamma a_\delta=a_{\gamma\delta}\phi_0(c_{\gamma,\delta}),\qquad a_e=e_2.
$$

When these can be solved, $\phi(s_\gamma h)=a_\gamma\phi_0(h)$ is a smooth global [homomorphism](../../../../../../homomorphism.md). They may prevent existence or allow several extensions with the same differential. Thus **a bracket-preserving [linear map](../../../../../../linear-map.md) gives local data; global integration requires the source's periods and, when present, its component relations to be respected**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
