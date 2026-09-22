<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the nonnegative Hodge-Laplacian convention from Question 4. The [Bochner-Weitzenbock formula for one-forms](../../../../../bochner-weitzenbock-formula-for-one-forms.md) is

$$
\boxed{\Delta\alpha=\nabla^*\nabla\alpha+\operatorname{Ric}\cdot\alpha.}
$$

Here $\nabla$ is the [Levi-Civita connection](../../../../../levi-civita-connection.md) induced on the [cotangent bundle](../../../../../cotangent-bundle.md), and the [rough Laplacian](../../../../../rough-laplacian.md) in a local orthonormal frame is

$$
\nabla^*\nabla\alpha=-\sum_i\bigl(\nabla_{e_i}\nabla_{e_i}\alpha-\nabla_{\nabla_{e_i}e_i}\alpha\bigr).
$$

It is the composition of [covariant derivative](../../../../../covariant-derivative.md) with its [formal adjoint](../../../../../formal-adjoint.md). The Ricci endomorphism is defined by $g(\operatorname{Ric}^{\sharp}X,Y)=\operatorname{Ric}(X,Y)$ and acts on one-forms by $(\operatorname{Ric}\cdot\alpha)(X)=\alpha(\operatorname{Ric}^{\sharp}X)$. The [musical isomorphism](../../../../../musical-isomorphism.md) defines $\alpha^{\sharp}$ by $g(\alpha^{\sharp},X)=\alpha(X)$. The associated scalar formula is

$$
\tfrac12\Delta|\alpha|^2=\langle\Delta\alpha,\alpha\rangle-|\nabla\alpha|^2-\operatorname{Ric}(\alpha^{\sharp},\alpha^{\sharp}).
$$

These signs make the integrated rough-Laplacian term $\|\nabla\alpha\|^2$ on a [closed manifold](../../../../../closed-manifold.md).

For a connected manifold, the full [Riemannian holonomy group](../../../../../riemannian-holonomy-group.md) at $p$ is the subgroup of $O(T_pM,g_p)$ consisting of parallel transports around all piecewise smooth loops based at $p$. Its natural action on $T_pM$ is the [holonomy representation](../../../../../holonomy-representation.md); it induces actions on cotangent spaces and all tensor spaces. The [holonomy representation](../../../../../holonomy-representation.md) is an [irreducible representation](../../../../../irreducible-representation.md) when it has no nonzero proper [invariant subspace](../../../../../invariant-subspace.md).

The [fundamental principle of Riemannian holonomy](../../../../../fundamental-principle-of-riemannian-holonomy.md) identifies parallel tensor fields with tensors at $p$ fixed by full holonomy. A parallel field returns to its value under every loop. Conversely, transport a fixed tensor along a path from $p$ to each point. Any two paths differ by a loop, so the result is independent of the path; local smooth [parallel transport](../../../../../parallel-transport.md) yields a smooth parallel field. Evaluation and construction are inverse. Full holonomy, not merely the contractible-loop subgroup, is required for this global correspondence.

On a compact manifold without boundary and with nonnegative [Ricci curvature](../../../../../ricci-curvature.md), a [harmonic one-form](../../../../../harmonic-one-form.md) satisfies the integrated Bochner identity

$$
0=\int_M\langle\Delta\alpha,\alpha\rangle\,d\mathrm{vol}_g
=\int_M\bigl(|\nabla\alpha|^2+\operatorname{Ric}(\alpha^{\sharp},\alpha^{\sharp})\bigr)\,d\mathrm{vol}_g.
$$

Both terms are nonnegative; therefore $\nabla\alpha=0$. This proves that [harmonic one-forms are parallel under nonnegative Ricci curvature](../../../../../harmonic-one-forms-are-parallel-under-nonnegative-ricci-curvature.md). Integration uses the Riemannian volume density and does not require an [orientation](../../../../../orientation-of-a-simplex.md).

If $n=\dim M\ge2$, a nonzero such form would give a nonzero fixed tangent vector via metric duality and hence a proper invariant line, contradicting irreducibility. This is precisely the [irreducible holonomy in dimension at least two has no parallel one-form](../../../../../irreducible-holonomy-in-dimension-at-least-two-has-no-parallel-one-form.md) criterion. Since the question permits harmonic representatives of all classes, it gives $b_1(M)=0$, where $b_1$ is the first [Betti number](../../../../../betti-number.md).

The covering $\pi:X\times T^k\to M$ is finite: its fibre over a point is a closed discrete subset of the compact total space and hence finite. Use the explicitly permitted equality of the Betti numbers of $M$ and its finite cover, in particular $b_1(X\times T^k)=b_1(M)=0$. This equality is a permission of this question, not a general theorem about finite covers.

The $k$ angular one-forms on $T^k$, pulled back to $X\times T^k$, represent linearly independent de Rham classes: their periods on the $k$ coordinate circles are the standard basis vectors. [exact differential forms](../../../../../exact-differential-form.md) have zero periods. Thus $b_1(X\times T^k)\ge k$, forcing $k=0$. Now $\pi:X\to M$ is a finite [universal covering map](../../../../../universal-cover.md) because $X$ is simply connected. The [fundamental group](../../../../../fundamental-group.md) acts freely and transitively on a fibre, or equivalently loop-lifting identifies its elements with the finite set of possible endpoints upstairs. Consequently the intended conclusion is

$$
\boxed{n\ge2\quad\Longrightarrow\quad k=0,\qquad |\pi_1(M)|=\deg\pi<\infty.}
$$

The printed statement needs the dimension qualification under the usual definition of irreducibility. Take the standard circle $M=S^1$, with $X$ a point, $k=1$, and the identity covering $X\times T^1\to S^1$. Its [Ricci curvature](../../../../../ricci-curvature.md) is zero. [parallel transport](../../../../../parallel-transport.md) fixes its global unit tangent, so its holonomy representation is the trivial representation on a one-dimensional real vector space, which is irreducible. The allowed Betti-number equality holds for this identity cover, yet

$$
\boxed{\pi_1(S^1)=\mathbb Z\text{ is infinite}.}
$$

Thus there is no proof of the unqualified literal assertion in dimension one. If “irreducible holonomy” is instead intended to exclude the one-dimensional trivial representation, the preceding intended proof applies. A connected zero-dimensional manifold is a point and has trivial [fundamental group](../../../../../fundamental-group.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 131](../../paper-131-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
