<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [principal bundle](../../../../../../principal-bundle.md) $\pi:E\to B$, the vertical space is $V_e=\ker d\pi_e$. A [principal connection](../../../../../../connection-principal-bundle.md) specifies smooth complements $T_eE=H_e\oplus V_e$ with $(R_g)_*H_e=H_{eg}$. Equivalently its Lie-algebra-valued connection one-form $\mathcal A$ satisfies $\mathcal A(\xi_E)=\xi$ and $R_g^*\mathcal A=\operatorname{Ad}_{g^{-1}}\mathcal A$. Every base vector has a unique [horizontal lift](../../../../../../horizontal-lift.md) because $d\pi:H_e\to T_{\pi(e)}B$ is an isomorphism. A base curve lifts from a chosen initial fiber point by solving $\mathcal A(\dot e)=0$; this defines [parallel transport](../../../../../../parallel-transport.md). Closed curves can give nontrivial [holonomy](../../../../../../holonomy.md), and failure of horizontal fields to close under brackets is measured by the [curvature of a principal connection](../../../../../../curvature-of-a-principal-connection.md).

For a smooth strictly convex [rigid body](../../../../../../rigid-body-dynamics.md), assume contact with the plane is unique and varies smoothly with orientation. Write a configuration as $(R,c_{\parallel})\in SO(3)\times\mathbb R^2$. Contact determines the reference point's height $h(R)$, so the full reference position is $c=(c_{\parallel},h(R))$. Let $r(R)$ be the spatial vector from that point to the contacting material point and let $\widehat\Omega=\dot R R^{-1}$ encode the spatial [angular velocity](../../../../../../angular-velocity.md). The instantaneous contact velocity is

$$
v_{\mathrm{contact}}=\dot c+\Omega\times r(R).
$$

The no-slip condition is its vanishing. Its vertical component follows already from differentiating contact: the normal component of the changing contact point along the body surface is zero, giving $\dot h=-(\Omega\times r)_z$. The two remaining equations are

$$
\dot c_{\parallel}=-(\Omega\times r(R))_{\parallel}.
$$

Translations of $c_{\parallel}$ define a free right $\mathbb R^2$ action, with quotient $SO(3)$. The [translational connection for a convex body rolling on a plane](../../../../../../translational-connection-for-a-convex-body-rolling-on-a-plane.md) is

$$
\boxed{\mathcal A=dc_{\parallel}+(\Omega\times r(R))_{\parallel}.}
$$

Here $\Omega$ denotes the vector-valued right [Maurer-Cartan form](../../../../../../maurer-cartan-form.md) on $SO(3)$. This one-form is invariant under translations and returns a translation vector on a vertical translation, so it satisfies both [principal connection](../../../../../../connection-principal-bundle.md) axioms. A prescribed orientation path has the unique rolling [horizontal lift](../../../../../../horizontal-lift.md)

$$
c_{\parallel}(t)=c_{\parallel}(0)-\int_0^t(\Omega(s)\times r(R(s)))_{\parallel}\,ds.
$$

This is a kinematic connection; inertia and gravity determine which of the allowed paths is dynamically realized.

For a sphere of radius $a$, $r=-a n$, where $n$ is the upward unit normal. The same no-slip condition gives $\dot c_{\parallel}=a\Omega\times n$. It leaves the component $\Omega\cdot n$ arbitrary. If one additionally forbids twisting about $n$, then $\Omega=n\times\dot c_{\parallel}/a$ and a plane path uniquely lifts to an orientation path by $\dot R=\widehat\Omega R$. This is the familiar $SO(3)$ [principal connection](../../../../../../connection-principal-bundle.md) over the plane; its horizontal lifts have noncommuting rotation generators and hence nonzero [curvature](../../../../../../curvature.md). No-slip alone does not supply that latter two-dimensional horizontal distribution. Corners or nonsmooth changes of contact require piecewise treatment rather than the smooth bundle construction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
