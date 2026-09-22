<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a connected smooth [Riemannian manifold](../../../../../riemannian-manifold.md) $(M,g)$ without boundary, let $I(M)$ be the group of all global [diffeomorphisms](../../../../../diffeomorphism.md) $f$ with $f^*g=g$, endowed with its [compact-open topology](../../../../../compact-open-topology.md). Equivalently these maps preserve the intrinsic distance; the [Myers-Steenrod theorem](../../../../../myers-steenrod-theorem.md) supplies smoothness of distance-preserving bijections and makes $I(M)$ a finite-dimensional [Lie group](../../../../../lie-group.md) acting smoothly. The group is metric-dependent: a topological manifold can carry a very symmetric metric or one with no continuous symmetries. Connectedness matters here. With infinitely many identical disconnected components, permutations of those components can produce a group which is not a finite-dimensional [Lie group](../../../../../lie-group.md).

An [isometry](../../../../../isometry.md) is determined by its value and derivative at one point. To prove this, suppose $f(p)=p$ and $df_p=I$. Preservation of the [Levi-Civita connection](../../../../../levi-civita-connection.md) gives

$$
f(\exp_p v)=\exp_p(df_pv)=\exp_pv
$$

where the [exponential map](../../../../../exponential-map-riemannian-geometry.md) is defined locally. Thus $f$ is the identity in a normal neighborhood of $p$. The set where its value and derivative agree with the identity is both closed and, by the same argument, open. Connectedness makes it all of $M$. No completeness is needed for this determination argument.

The stabilizer $I(M)_p$ consequently acts faithfully and orthogonally on $T_pM$, so embeds in $O(n)$. More generally an [isometry](../../../../../isometry.md) takes a chosen [orthonormal frame](../../../../../orthonormal-frame-in-spacetime.md) at $p$ to one at its image point, providing an injective map into the [orthonormal frame bundle](../../../../../orthonormal-frame-bundle.md). It is a smooth embedding, and the full [isometry](../../../../../isometry.md) action is proper. The orbit-stabilizer dimension formula therefore gives

$$
\boxed{\dim I(M)\leq n+\frac{n(n-1)}2=\frac{n(n+1)}2.}
$$

Isotropy is compact. If $M$ is compact then $I(M)$ itself is compact, by the same frame description or Arzela-Ascoli applied to [isometries](../../../../../isometry.md) and their inverses. Properness also means that the quotient by [isometries](../../../../../isometry.md) has well-controlled local orbit structure, even though orbit dimensions may vary.

The infinitesimal equation is the [Killing equation](../../../../../killing-equation.md). Differentiating $f_t^*g=g$ at zero gives

$$
\mathcal L_Xg=0,\qquad \nabla_iX_j+\nabla_jX_i=0.
$$

Conversely a vector field satisfying this equation has local flows preserving the metric. A global one-parameter subgroup requires the field to be complete. On a geodesically complete manifold every [Killing field](../../../../../killing-vector-field.md) is complete: its length is constant along each of its own trajectories, so a finite-time trajectory has bounded speed and stays in a closed bounded ball. The [Hopf-Rinow theorem](../../../../../hopf-rinow-theorem.md) makes that ball compact, and the [ordinary differential equation](../../../../../ordinary-differential-equation.md) can then be continued. The caveat is real: on the Euclidean interval $(0,1)$, the field $\partial_x$ is Killing but its translations are not globally defined for all time. This illustrates [Killing fields on incomplete manifolds need not generate global isometries](../../../../../killing-fields-on-incomplete-manifolds-need-not-generate-global-isometries.md).

The [Killing transport](../../../../../killing-transport.md) identities determine a [Killing field](../../../../../killing-vector-field.md) from $X(p)$ and the skew-adjoint map $(\nabla X)_p$. Along a [geodesic](../../../../../geodesic.md) the field is a [Jacobi field](../../../../../jacobi-field.md), so uniqueness for its second-order [differential equation](../../../../../differential-equation-split.md) propagates these [initial data](../../../../../initial-data-in-general-relativity.md). They have $n+n(n-1)/2$ components, reproducing the dimension bound infinitesimally. The important distinction on an incomplete manifold is between all local Killing solutions and the [Lie algebra](../../../../../lie-algebra-split.md) of complete global [isometry](../../../../../isometry.md) flows.

In dimension three the bound is six, and rotational isotropy gives stronger information. The [Lie subalgebras](../../../../../lie-subalgebra.md) of $\mathfrak{so}(3)$ have dimensions zero, one or three: identifying the bracket with the cross product, a two-plane is not closed under brackets. Suppose $\dim I(M)=5$. Since an orbit has dimension at most three, its stabilizer would have dimension at least two, and hence exactly three. Its connected isotropy acts as all of $SO(3)$ on the tangent space. But the orbit tangent space is invariant under that action and would have dimension $5-3=2$, impossible because the standard rotational representation is irreducible. Therefore **dimension five cannot occur**.

If the dimension is six, each orbit has dimension three and each stabilizer dimension three. All orbits are open, so connectedness makes the action transitive. At each point the isotropy is transitive on tangent two-planes, forcing [sectional curvature](../../../../../sectional-curvature.md) to be independent of the plane; transitivity makes its value independent of the point. Thus a maximally symmetric connected [three-manifold](../../../../../3-manifold.md) has [constant sectional curvature](../../../../../constant-sectional-curvature.md). Homogeneous [Riemannian manifolds](../../../../../riemannian-manifold.md) are complete, so its [simply connected](../../../../../simply-connected-space.md) cover is the round sphere, [Euclidean space](../../../../../euclidean-norm.md) or [hyperbolic space](../../../../../hyperbolic-space.md) after normalization. Conversely these three [simply connected](../../../../../simply-connected-space.md) metrics attain dimension six:

$$
I(S^3)=O(4),\qquad I(\mathbb R^3)=\mathbb R^3\rtimes O(3),\qquad
I(\mathbb H^3)=O^+(3,1).
$$

Here $O^+(3,1)$ preserves the chosen sheet of the hyperboloid; it includes orientation-reversing hyperbolic [isometries](../../../../../isometry.md). Constant curvature alone does not imply that a quotient retains six-dimensional global symmetry.

Dimension four likewise forces transitivity: stabilizer dimension three would give a one-dimensional invariant orbit tangent space, again impossible for full rotational isotropy. The stabilizer thus has dimension one and the orbits are three-dimensional. Typical four-dimensional [isometry groups](../../../../../isometry-group.md) occur for $S^2\times\mathbb R$ and $\mathbb H^2\times\mathbb R$, where the factor groups have dimensions three and one. The usual Nil metric has three translation symmetries and one rotational isotropy symmetry. In centred Heisenberg coordinates it is

$$
g=dx^2+dy^2+\bigl(dt+\tfrac12(y\,dx-x\,dy)\bigr)^2,
$$

which exhibits the horizontal rotations. Its distinct vertical and horizontal Ricci eigenvalues bound continuous isotropy by that rotation group, so its full [isometry](../../../../../isometry.md) dimension is four. Standard metrics on $\widetilde{SL_2(\mathbb R)}$ and nonround Berger spheres also have dimension four. The standard Sol geometry has a three-dimensional translation group and only finite isotropy, giving dimension three. These examples show how a preferred vertical direction reduces rotational symmetry.

The [isometry dimensions in dimension three](../../../../../isometry-dimensions-in-dimension-three.md) are precisely $0,1,2,3,4,6$, all realizable. A compact [hyperbolic three-manifold](../../../../../hyperbolic-three-manifold.md) gives zero; the product of a circle and a closed hyperbolic surface gives one. For dimension two take $T^2\times(0,1)$ with

$$
g=dt^2+e^{2t}\,dx^2+e^{4t}\,dy^2.
$$

Its [scalar curvature](../../../../../scalar-curvature.md) is the constant $-14$, but its Ricci eigenvalues are the distinct constants $-3,-6,-5$ in the two horizontal directions and the vertical direction. Hence connected isotropy is trivial and possible [isometries](../../../../../isometry.md) preserve these line distributions. A local [isometry](../../../../../isometry.md) preserving them has $t'=t+c$ and would require constant dilations $e^{-c}$ and $e^{-2c}$ of the two circle coordinates. A global circle [diffeomorphism](../../../../../diffeomorphism.md) with such a constant dilation has degree $\pm1$, forcing $c=0$. The identity component is therefore exactly the two circle translations. A flat three-torus gives dimension three; $S^2\times\mathbb R$ gives four; a [simply connected](../../../../../simply-connected-space.md) constant-curvature model gives six. This construction distinguishes local homogeneity from the smaller global [isometry group](../../../../../isometry-group.md).

For quotients, let a complete [simply connected](../../../../../simply-connected-space.md) [Riemannian manifold](../../../../../riemannian-manifold.md) $X$ cover $M=X/\Gamma$. Every [isometry](../../../../../isometry.md) of $M$ lifts to an [isometry](../../../../../isometry.md) of $X$ which normalizes the [deck transformation group](../../../../../deck-transformation-group.md). Conversely, every normalizing [isometry](../../../../../isometry.md) descends. Two lifts differ by a [deck transformation](../../../../../deck-transformation.md), giving the [isometry group of a Riemannian quotient](../../../../../isometry-group-of-a-riemannian-quotient.md) formula

$$
\boxed{I(X/\Gamma)=N_{I(X)}(\Gamma)/\Gamma.}
$$

Thus one should not replace the [isometry group](../../../../../isometry-group.md) of a quotient by that of its model geometry. For a [flat torus](../../../../../flat-torus.md), for example,

$$
I(\mathbb R^3/\Lambda)=(\mathbb R^3/\Lambda)\rtimes\{R\in O(3):R\Lambda=\Lambda\}.
$$

The second factor is finite, whereas translations give the three-dimensional identity component.

There is a useful curvature test for [compact manifolds](../../../../../compact-manifold.md). Contracting and differentiating the [Killing equation](../../../../../killing-equation.md) gives $\nabla^*\nabla X=\operatorname{Ric}(X)$, with the nonnegative rough-Laplacian convention. Integration yields the [integrated Bochner identity for Killing fields](../../../../../bochner-identity-for-killing-vector-fields.md)

$$
\int_M|\nabla X|^2\,dV=\int_M\operatorname{Ric}(X,X)\,dV.
$$

If [Ricci curvature](../../../../../ricci-curvature.md) is negative definite, no nonzero [Killing field](../../../../../killing-vector-field.md) exists. The compact [isometry group](../../../../../isometry-group.md) then has dimension zero and is finite. This explains why closed hyperbolic manifolds have finite global symmetry, despite the six-dimensional [isometry group](../../../../../isometry-group.md) of their [universal cover](../../../../../universal-cover.md). Compactness is essential to this conclusion.

For a compact [flat Riemannian manifold](../../../../../flat-manifold.md), the same identity makes every [Killing field](../../../../../killing-vector-field.md) parallel. Parallel fields are exactly the vectors fixed by linear holonomy. Therefore

$$
\boxed{\dim I(M)_0=\dim(\mathbb R^3)^{\operatorname{Hol}(M)}.}
$$

Applied to the six flat types of Question 1, this gives dimensions three for the [torus](../../../../../torus.md), one for each of the four nontrivial cyclic types, and zero for the [Hantzsche-Wendt manifold](../../../../../hantzsche-wendt-manifold.md). These are identity-component dimensions; disconnected finite symmetries can still be present. Local curvature symmetry, global deck-group constraints, and completeness thus play different roles in determining the [isometry group](../../../../../isometry-group.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
