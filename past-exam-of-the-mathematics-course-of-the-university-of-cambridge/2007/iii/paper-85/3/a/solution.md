<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let a finite or compact group $G$ act linearly on a real space $V$, and let $\dot x=F(x,\mu)$ be a smooth [equivariant dynamical system](../../../../../../equivariant-dynamical-system.md): $F(gx,\mu)=gF(x,\mu)$. Assume $F(0,\mu)=0$. The representation is an [absolutely irreducible real representation](../../../../../../absolutely-irreducible-real-representation.md) when its complexification is irreducible; equivalently, every real linear operator commuting with $G$ is a scalar multiple of the identity. Consequently the [linearization](../../../../../../linearization.md) at the trivial branch is $D_xF(0,\mu)=\alpha(\mu)I$. A generic steady-state crossing has $\alpha(0)=0$ and $\alpha'(0)\ne0$, with stable noncritical directions removed by a [centre manifold](../../../../../../center-manifold.md) if this is a reduction of a larger system.

The [isotropy group](../../../../../../stabilizer-subgroup.md) of a vector $x$ is $\Sigma_x=\{g\in G:gx=x\}$. For a subgroup $\Sigma$, its [fixed-point subspace of a group action](../../../../../../fixed-point-subspace-of-a-group-action.md) is $\operatorname{Fix}(\Sigma)=\{x:\sigma x=x\text{ for every }\sigma\in\Sigma\}$. Its [normaliser](../../../../../../normalizer.md) is

$$
N_G(\Sigma)=\{g\in G:g\Sigma g^{-1}=\Sigma\}.
$$

The [normaliser](../../../../../../normalizer.md) preserves $\operatorname{Fix}(\Sigma)$, and $N_G(\Sigma)/\Sigma$ describes its residual symmetry. A steady-state [axial subgroup](../../../../../../axial-subgroup.md) is an actual isotropy subgroup with $\dim_{\mathbb R}\operatorname{Fix}(\Sigma)=1$.

The [equivariant branching lemma](../../../../../../equivariant-branching-lemma.md) states that, under the smoothness, equivariance, absolute irreducibility, and transverse scalar-[eigenvalue](../../../../../../eigenvalue.md) crossing hypotheses above, each conjugacy class of axial isotropy subgroup gives a branch of nonzero [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) in its fixed-point line through $(0,0)$. The generic leading nonlinear coefficient determines which parameter side the branch occupies and whether it is transcritical-like or pitchfork-like; the theorem does not assert that these branches are stable or exhaust every possible branch. The usual nondegeneracy condition excludes a vanishing leading nonlinear coefficient. Conjugate subgroups produce symmetry-related copies of a branch, rather than new isotropy types.

To explain the dynamical role of the [fixed-point subspaces of a group action](../../../../../../fixed-point-subspace-of-a-group-action.md), if $x$ is fixed by $\Sigma$, then $\sigma F(x,\mu)=F(\sigma x,\mu)=F(x,\mu)$ for every $\sigma\in\Sigma$. Thus the vector field is tangent to that subspace, and uniqueness makes it flow invariant. On a fixed-point line one solves a scalar [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) equation and determines radial stability. Stability in the full space additionally requires all transverse [eigenvalues](../../../../../../eigenvalue.md) to be stable. Higher-dimensional fixed-point spaces support their own restricted dynamics and may contain symmetry-constrained connecting orbits.

Finally, the [normalizer action determines axial branch parity](../../../../../../normalizer-action-determines-axial-branch-parity.md): if $N_G(\Sigma)/\Sigma$ contains an element acting as $x\mapsto-x$ on the fixed line, its scalar vector field must be odd, so a generic cubic term gives a [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md). If that residual sign reversal is absent, a quadratic term is permitted and can give a transcritical-like branch. This is why fixed-space dimension alone does not determine either the branch type or its full stability.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
