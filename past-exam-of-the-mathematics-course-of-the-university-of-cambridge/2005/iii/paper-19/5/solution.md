<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A smooth manifold alone has no distinguished notion of an [isometry](../../../../../isometry.md); one must first choose a [Riemannian metric](../../../../../riemannian-metric.md) $g$. We therefore interpret the essay as concerning a smooth connected [Riemannian manifold](../../../../../riemannian-manifold.md) $(M,g)$. Its [isometry group](../../../../../isometry-group.md) consists of diffeomorphisms $f$ with $f^*g=g$. In coordinates this is

$$
g_{ab}(f(x))\,\partial_i f^a\,\partial_j f^b=g_{ij}(x).
$$

An [isometry](../../../../../isometry.md) preserves lengths, distances, the Levi-Civita connection, [geodesics](../../../../../geodesic.md) and all curvature tensors. The [Myers-Steenrod theorem](../../../../../myers-steenrod-theorem.md) ensures that the [group](../../../../../group-split.md) is a finite-dimensional [Lie group](../../../../../lie-group.md) acting smoothly, and that even distance-preserving bijections have the required smoothness.

The crucial rigidity is determination by one first jet. An [isometry](../../../../../isometry.md) fixing $p$ satisfies

$$
f(\exp_p v)=\exp_p(df_pv)
$$

wherever the exponential chart is defined. If also $df_p=I$, it is the identity on a neighborhood. Continuing this equality through overlapping exponential neighborhoods proves it on connected $M$. Therefore the [isotropy group](../../../../../stabilizer-subgroup.md) at $p$ embeds in $O(T_pM,g_p)$. Its dimension is at most $n(n-1)/2$, while an orbit has dimension at most $n$. Consequently

$$
\boxed{\dim\operatorname{Isom}(M,g)\le\frac{n(n+1)}2;\qquad n=3\text{ gives }\dim\operatorname{Isom}(M,g)\le6.}
$$

On a [compact manifold](../../../../../compact-manifold.md) the [group](../../../../../group-split.md) is compact. Indeed distance preservation makes a family of [isometries](../../../../../isometry.md) equicontinuous; compactness and the same argument for their inverses give subsequential limits which are inverse distance-preserving bijections. Smoothness and the Lie-group structure then follow from [Myers-Steenrod theorem](../../../../../myers-steenrod-theorem.md).

Infinitesimal [isometries](../../../../../isometry.md) are [Killing vector fields](../../../../../killing-vector-field.md). Differentiating $f_t^*g=g$ at zero gives

$$
\mathcal L_Xg=0,\qquad \nabla_iX_j+\nabla_jX_i=0.
$$

On a complete [Riemannian manifold](../../../../../riemannian-manifold.md) these fields have complete flows and constitute the [Lie algebra](../../../../../lie-algebra-split.md) of the [isometry group](../../../../../isometry-group.md); on an incomplete manifold one must retain only fields whose flows are globally defined. A [Killing vector field](../../../../../killing-vector-field.md) is fixed by its value and its skew derivative at one point, consistent with the same dimension bound. Along a [geodesic](../../../../../geodesic.md), its restriction is a Jacobi field, so local infinitesimal data propagate rigidly.

In dimension three there is no independent Weyl curvature tensor: the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) is determined by the [Ricci tensor](../../../../../ricci-tensor.md). Large isotropy therefore strongly constrains the geometry. If the full dimension six is attained, the [group](../../../../../group-split.md) is transitive with three-dimensional isotropy. That isotropy rotates all tangent two-planes transitively, forcing equal sectional curvatures at each point; transitivity makes the value constant. The simply connected complete models are the round $S^3$, Euclidean $\mathbb R^3$ and hyperbolic $\mathbb H^3$. Their [groups](../../../../../group-split.md) are respectively $O(4)$, $\mathbb R^3\rtimes O(3)$ and $O^+(3,1)$, all of dimension six. The orientation-preserving hyperbolic [group](../../../../../group-split.md) is $PSL_2(\mathbb C)$.

The standard [Thurston geometries](../../../../../thurston-geometry.md) show how symmetry drops when a preferred direction is present:

$$
\begin{array}{c|c|c}
\text{model}&\dim\operatorname{Isom}&\dim\text{continuous isotropy}\\\hline
S^3,\ \mathbb R^3,\ \mathbb H^3&6&3\\
S^2\times\mathbb R,\ \mathbb H^2\times\mathbb R&4&1\\
\mathrm{Nil},\ \widetilde{SL_2(\mathbb R)}&4&1\\
\mathrm{Sol}&3&0
\end{array}
$$

For the product models, the [surface](../../../../../topological-surface.md) factor has a three-dimensional [isometry group](../../../../../isometry-group.md), and translations along the line add one parameter. For Nil and the universal covering of $SL_2(\mathbb R)$ with their standard geometric metrics, a three-dimensional transitive [group](../../../../../group-split.md) is enlarged by a circle of isotropy. The Sol metric

$$
ds^2=e^{2w}du^2+e^{-2w}dv^2+dw^2
$$

is preserved by $(u,v,w)\mapsto(u_0+e^{-t}u,v_0+e^tv,w+t)$, giving three continuous parameters; its continuous isotropy is trivial because the distinguished expanding and contracting directions cannot be rotated into each other. Additional discrete symmetries may still occur. These dimensions refer to the model metrics, not arbitrary left-invariant perturbations.

A quotient generally has fewer global [isometries](../../../../../isometry.md) than its local model. If $X$ is the complete simply connected [universal cover](../../../../../universal-cover.md) and $M=X/\Gamma$, the [isometry group of a Riemannian quotient](../../../../../isometry-group-of-a-riemannian-quotient.md) is

$$
\boxed{\operatorname{Isom}(M)=N_{\operatorname{Isom}(X)}(\Gamma)/\Gamma.}
$$

To prove this, lift an [isometry](../../../../../isometry.md) to the [universal cover](../../../../../universal-cover.md). Conjugating a deck transformation by the lift again gives a deck transformation, so the lift normalizes $\Gamma$. Conversely a normalizing [isometry](../../../../../isometry.md) descends, and two lifts differ by a deck transformation. A flat three-torus retains its three-dimensional translation [group](../../../../../group-split.md), with additional discrete lattice symmetries. A round spherical quotient retains only the normalizer of its finite deck [group](../../../../../group-split.md); the full six-dimensional [group](../../../../../group-split.md) does not automatically descend.

For a closed [hyperbolic three-manifold](../../../../../hyperbolic-three-manifold.md), there are no nonzero [Killing vector fields](../../../../../killing-vector-field.md). The integrated Killing identity is

$$
\int_M|\nabla X|^2\,dV=\int_M\operatorname{Ric}(X,X)\,dV=-2\int_M|X|^2\,dV.
$$

Both nonnegative terms must vanish. The compact [isometry group](../../../../../isometry-group.md) is therefore zero-dimensional and hence finite. The [Mostow rigidity theorem](../../../../../mostow-rigidity-theorem.md) additionally says that isomorphisms between the [fundamental groups](../../../../../fundamental-group.md) of complete finite-volume hyperbolic three-manifolds are induced by unique hyperbolic [isometries](../../../../../isometry.md); this fixes the complete hyperbolic metric up to [isometry](../../../../../isometry.md) and contrasts with the moduli of flat [tori](../../../../../torus.md). An arbitrary smooth three-manifold need not admit a single homogeneous metric: prime decomposition and [torus](../../../../../torus.md) splitting may lead to several geometric pieces. Thus **local homogeneous symmetry, global quotient symmetry and the chosen metric must be distinguished** when discussing [isometries](../../../../../isometry.md) in dimension three.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
