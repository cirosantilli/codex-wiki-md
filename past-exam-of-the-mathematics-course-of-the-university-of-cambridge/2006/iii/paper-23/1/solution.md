<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the nonnegative scalar [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) $\Delta=-\operatorname{div}\nabla$ on a closed compact [Riemannian manifold](../../../../../riemannian-manifold.md), and include every [eigenvalue](../../../../../eigenvalue.md) with its multiplicity. The [spectrum](../../../../../spectrum-functional-analysis.md) contains substantial global geometric information, but generally does not determine the [Riemannian metric](../../../../../riemannian-metric.md) up to [isometry](../../../../../isometry.md). Specifying the operator and its domain matters: the spectrum on functions is different information from the spectra of the [Hodge Laplacian](../../../../../hodge-laplacian.md) on differential forms, and a boundary requires fixed [boundary conditions](../../../../../boundary-condition.md).

The [Weyl law](../../../../../weyl-law.md) makes dimension and volume audible. If $N(\lambda)$ counts [eigenvalues](../../../../../eigenvalue.md) at most $\lambda$, then

$$
N(\lambda)\sim\frac{\omega_d\operatorname{Vol}(M)}{(2\pi)^d}\lambda^{d/2},
$$

where $\omega_d$ is the volume of the Euclidean unit ball. Thus the growth exponent recovers $d$, and its leading coefficient recovers $\operatorname{Vol}(M)$. The multiplicity of zero gives the number of connected components: a function in the kernel has $\int|\nabla f|^2=0$ and hence is constant on each component.

More detailed invariants come from the [heat trace](../../../../../heat-trace.md), which is determined directly by the [spectrum](../../../../../spectrum-functional-analysis.md):

$$
Z_M(t)=\sum_j e^{-t\lambda_j}\sim(4\pi t)^{-d/2}\left(a_0+a_1t+a_2t^2+\cdots\right).
$$

The first [heat invariants](../../../../../heat-invariants.md) for a closed manifold are

$$
a_0=\operatorname{Vol}(M),\qquad a_1=\frac16\int_M R\,dV,\qquad a_2=\frac1{360}\int_M(5R^2-2|\operatorname{Ric}|^2+2|\operatorname{Rm}|^2)\,dV.
$$

Here $R$ is [scalar curvature](../../../../../scalar-curvature.md), $\operatorname{Ric}$ the [Ricci curvature](../../../../../ricci-curvature.md), and $\operatorname{Rm}$ the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md). A divergence term in the local coefficient integrates to zero on a closed manifold. The expansion supplies further integrated curvature expressions, rather than a pointwise curvature map.

On a closed surface, $R=2K$, $|\operatorname{Ric}|^2=2K^2$ and $|\operatorname{Rm}|^2=4K^2$, so the same coefficients become

$$
a_0=A,\qquad a_1=\frac13\int_MK\,dA,\qquad a_2=\frac1{15}\int_MK^2\,dA.
$$

The [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives $\int K\,dA=2\pi\chi(M)$; hence the constant term of the [heat trace](../../../../../heat-trace.md) is $\chi(M)/6$. In particular the [Euler characteristic](../../../../../euler-characteristic.md), and for a connected orientable surface its [genus](../../../../../genus-of-a-surface.md), are spectrally determined. There is even [spectral determination of hyperbolic curvature on a surface](../../../../../spectral-determination-of-hyperbolic-curvature-on-a-surface.md): if this spectrum agrees with that of a curvature-$-1$ surface, the coefficients give $\int K=-A$ and $\int K^2=A$, whence

$$
\int_M(K+1)^2\,dA=A-2A+A=0.
$$

Thus $K=-1$ everywhere. This determines local curvature, while leaving room for globally nonisometric [hyperbolic surfaces](../../../../../hyperbolic-surface.md).

Geodesic information is also accessible in important settings. For closed [hyperbolic surfaces](../../../../../hyperbolic-surface.md), the [Selberg trace formula](../../../../../selberg-trace-formula.md) makes the scalar [spectrum](../../../../../spectrum-functional-analysis.md) equivalent to the unmarked [length spectrum](../../../../../length-spectrum.md) with its appropriate multiplicities. This does not supply a [marked length spectrum](../../../../../marked-length-spectrum.md): it does not identify which group element or intersecting curve has a given length. For general manifolds, one must not simply assert this equivalence; the singularities of the wave trace can be affected by degeneracies and cancellations.

The historic development separates these positive results from the inverse problem. Weyl's 1911 eigenvalue asymptotics established the leading geometric information. The [Minakshisundaram-Pleijel heat expansion](../../../../../heat-kernel-expansion.md) of 1949 brought local curvature into the short-time analysis. In 1964 Milnor exhibited nonisometric [flat tori](../../../../../flat-torus.md) in dimension sixteen with identical scalar spectra, showing that all [eigenvalues](../../../../../eigenvalue.md) together need not recover the metric. Kac's 1966 question about a vibrating drum popularized the corresponding inverse problem for planar domains. Vignéras's 1980 hyperbolic examples and the [Sunada theorem](../../../../../sunada-theorem.md) of 1985 extended the supply of counterexamples; the latter turns [Gassmann equivalence](../../../../../gassmann-equivalence.md) of finite subgroups into a geometric construction. The four-dimensional [tetracode length-isospectral lattice construction](../../../../../tetracode-length-isospectral-lattice-construction.md) and the planar examples of Gordon, Webb and Wolpert in 1992 made nonuniqueness explicit in smaller dimensions and in the original drum setting.

Nor is scalar [isospectrality](../../../../../isospectral-manifolds.md) a universal topological invariant strong enough to determine the manifold. For example, [Tetra and Didi](../../../../../tetra-and-didi.md) are scalar-isospectral closed orientable flat three-manifolds with first [Betti numbers](../../../../../betti-number.md) one and zero. Their topology therefore differs. The spectra of all [Hodge Laplacians](../../../../../hodge-laplacian.md) would detect these [Betti numbers](../../../../../betti-number.md) through the dimensions of their zero eigenspaces, illustrating the extra information obtained by changing the operator. **Dimension, volume and many integrated invariants are determined; the full metric and, in general, the topology are not.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
