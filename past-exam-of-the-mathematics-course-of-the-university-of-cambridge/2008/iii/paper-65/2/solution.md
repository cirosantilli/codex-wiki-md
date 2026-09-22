<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [Lie group](../../../../../lie-group.md) $G$, [Left translation on a Lie group](../../../../../left-and-right-translation-on-a-lie-group.md) and [right translation on a Lie group](../../../../../left-and-right-translation-on-a-lie-group.md) are the [diffeomorphisms](../../../../../diffeomorphism.md) $L_g(h)=gh$ and $R_g(h)=hg$. Their differentials identify the tangent space at the identity with every tangent space. Translating a basis $e_a$ of the [Lie algebra](../../../../../lie-algebra-split.md) gives global [left-invariant vector fields](../../../../../left-invariant-vector-field.md) $E_a(g)=(dL_g)_e e_a$ and [right-invariant vector fields](../../../../../right-invariant-vector-field.md) $F_a(g)=(dR_g)_e e_a$. Left and right translations commute. If $[e_a,e_b]=c^c{}_{ab}e_c$, then

$$
[E_a,E_b]=c^c{}_{ab}E_c,\qquad [F_a,F_b]=-c^c{}_{ab}F_c.
$$

The opposite sign for the right-invariant frame is essential.

Define an [affine connection](../../../../../affine-connection.md) $\nabla^-$ by declaring the $E_a$ parallel. Explicitly, $\nabla^-_X(f^aE_a)=X(f^a)E_a$. Its [curvature form of a connection](../../../../../curvature-form.md) vanishes, since successive derivatives of the component functions satisfy the vector-field commutator identity. Its [torsion tensor](../../../../../torsion-tensor.md) is

$$
T^-(E_a,E_b)=\nabla^-_{E_a}E_b-\nabla^-_{E_b}E_a-[E_a,E_b]=-[E_a,E_b].
$$

Similarly, declaring the $F_a$ parallel gives another flat [affine connection](../../../../../affine-connection.md) $\nabla^+$, with $T^+(F_a,F_b)=-[F_a,F_b]$. In a left-invariant frame the latter connection obeys

$$
\nabla^+_XY=[X,Y].
$$

To see this, express $E_a=F_{\operatorname{Ad}_g e_a}$. Along $g\exp(t e_b)$, differentiation of $\operatorname{Ad}_{g\exp(t e_b)}e_a$ gives $\operatorname{Ad}_g[e_b,e_a]$, producing the displayed bracket. Consequently $T^+(X,Y)=[X,Y]$ for left-invariant $X,Y$. These are the [flat translation connections on a Lie group](../../../../../flat-translation-connections-on-a-lie-group.md). They have opposite torsion; if $G$ is Abelian, both torsion tensors vanish and the two connections coincide. The phrase “with torsion” does not mean nonzero torsion for Abelian groups.

The average $\nabla^0=(\nabla^-+\nabla^+)/2$ is again an [affine connection](../../../../../affine-connection.md) and satisfies $\nabla^0_XY=\frac12[X,Y]$ for left-invariant fields. Its [torsion tensor](../../../../../torsion-tensor.md) is zero. With the curvature convention $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$, the [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
\begin{aligned}
R^0(X,Y)Z
&=\frac14\bigl([X,[Y,Z]]-[Y,[X,Z]]\bigr)-\frac12[[X,Y],Z]\\
&=-\frac14[[X,Y],Z].
\end{aligned}
$$

Define the [Ricci tensor](../../../../../ricci-tensor.md) by $\operatorname{Ric}(X,Y)=\operatorname{Tr}(Z\mapsto R(Z,X)Y)$. Since $[[Z,X],Y]=\operatorname{ad}_Y\operatorname{ad}_X Z$, this gives

$$
\boxed{R^0(X,Y)Z=-\frac14[[X,Y],Z],\qquad
\operatorname{Ric}^0(X,Y)=-\frac14K(X,Y),}
$$

where $K(X,Y)=\operatorname{Tr}(\operatorname{ad}_X\operatorname{ad}_Y)$ is the [Killing form](../../../../../killing-form.md). Thus the [canonical torsion-free connection on a Lie group](../../../../../canonical-torsion-free-connection-on-a-lie-group.md) is generally curved. Its exact flatness criterion is $[[\mathfrak g,\mathfrak g],\mathfrak g]=0$: Abelian and two-step nilpotent groups are exceptions. A vanishing [Ricci tensor](../../../../../ricci-tensor.md) alone does not prove flatness.

For a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), the [Killing form](../../../../../killing-form.md) is nondegenerate. Its adjoint invariance gives $K([X,Y],Z)+K(Y,[X,Z])=0$, so translating it defines a [bi-invariant pseudo-Riemannian metric](../../../../../bi-invariant-pseudo-riemannian-metric.md) $g_K$. For left-invariant fields,

$$
(\nabla^0_Xg_K)(Y,Z)=-\frac12\bigl(K([X,Y],Z)+K(Y,[X,Z])\bigr)=0.
$$

A metric-compatible [torsion-free connection](../../../../../torsion-free-connection.md) is uniquely the [Levi-Civita connection](../../../../../levi-civita-connection.md); therefore $\nabla^0$ is its Levi-Civita connection. Moreover,

$$
\boxed{\operatorname{Ric}(g_K)=-\frac14g_K.}
$$

The special feature is a canonical nondegenerate metric and an [Einstein manifold](../../../../../einstein-manifold.md) structure. The metric need not be positive definite: noncompact semisimple groups generally require indefinite signature. For compact semisimple groups, using $-K$ gives a [bi-invariant Riemannian metric](../../../../../bi-invariant-riemannian-metric.md) with $\operatorname{Ric}=\frac14g_{-K}$ instead.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
