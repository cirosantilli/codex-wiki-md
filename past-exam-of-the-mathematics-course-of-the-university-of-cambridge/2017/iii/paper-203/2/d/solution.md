<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Using the usual [zero-boundary Sobolev space](../../../../../../zero-boundary-sobolev-space.md) convention,

$$
H_0^1(D)=\overline{C_c^\infty(D)}^{\,H^1(D)},\qquad \|u\|_{H^1(D)}^2=\int_D(|u|^2+|\nabla u|^2)\,dA,
$$

where [weak derivatives](../../../../../../weak-derivative.md) define $H^1(D)$ and $C_c^\infty(D)$ is the [space of test functions](../../../../../../space-of-test-functions.md). In the [Gaussian free field](../../../../../../gaussian-free-field.md) convention, the same notation often denotes the [Dirichlet energy space](../../../../../../dirichlet-energy-space.md), the completion in the [gradient](../../../../../../gradient.md) [norm](../../../../../../norm.md) alone. On bounded [domains](../../../../../../domain-mathematical-analysis.md) the [Poincaré inequality](../../../../../../poincare-inequality.md) makes the two definitions equivalent; on unbounded [domains](../../../../../../domain-mathematical-analysis.md) one must distinguish them. The following gradient-pairing argument applies in either setting whenever the energy completion is realized as weak functions.

Identify $H_{\mathrm{supp}}=H_0^1(U)$ with a [vector subspace](../../../../../../vector-subspace.md) of $H_0^1(D)$ by [zero extension of H01](../../../../../../zero-extension-of-h01.md). Approximating by [test functions](../../../../../../test-function.md) in $U$ shows that this is an [isometric embedding](../../../../../../isometric-embedding.md) in the inhomogeneous [Sobolev norm](../../../../../../sobolev-norm.md) and also in the [Dirichlet inner product](../../../../../../dirichlet-inner-product.md) [norm](../../../../../../norm.md). In particular, arbitrary irregularity of $\partial U$ causes no additional [boundary](../../../../../../boundary-of-a-set.md) term.

Define

$$
H_{\mathrm{harm}}=\{h\in H_0^1(D):\Delta h=0\text{ in distributions on }U\}.
$$

These are [weakly harmonic Sobolev functions](../../../../../../weakly-harmonic-sobolev-function.md). For $\phi\in C_c^\infty(U)$, [integration by parts](../../../../../../integration-by-parts.md) in the weak sense gives $\int_U\nabla h\cdot\nabla\phi\,dA=0$. If $u\in H_{\mathrm{supp}}$, choose $\phi_n\in C_c^\infty(U)$ converging to $u$ in $H^1(U)$, or in energy for the homogeneous convention. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
(h,u)_{\nabla,D}=\lim_{n\to\infty}(h,\phi_n)_{\nabla,D}=0.
$$

Hence the [orthogonality of supported and harmonic Dirichlet functions](../../../../../../orthogonality-of-supported-and-harmonic-dirichlet-functions.md) is

$$
\boxed{H_{\mathrm{supp}}\perp H_{\mathrm{harm}}.}
$$

Both are linear [vector subspaces](../../../../../../vector-subspace.md). In the inhomogeneous convention they are closed: the first is the isometric image of a complete space, and the second is the intersection of the kernels of the [linear functionals](../../../../../../linear-functional.md) $h\mapsto(h,\phi)_\nabla$. No spanning assertion is needed. The PDF contains this [orthogonality](../../../../../../orthogonal-vectors.md) statement; the TeX has badly corrupted it into an assertion about openness.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
