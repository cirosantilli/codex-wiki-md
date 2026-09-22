<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use natural units and the [Minkowski metric](../../../../../minkowski-metric.md) $\eta_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$. For the [real scalar field](../../../../../real-scalar-field.md), choose $\mathcal L_0=\frac12\partial_\mu\phi\partial^\mu\phi-\frac12m^2\phi^2$. The conjugate momentum is $\pi=\dot\phi$. Under an active translation $\delta\phi=\varepsilon a^\nu\partial_\nu\phi$, the density changes by $\delta\mathcal L_0=\varepsilon\partial_\mu(a^\mu\mathcal L_0)$. The [Noether theorem](../../../../../noether-theorem.md) therefore gives the [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md)

$$
T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi-\eta^{\mu\nu}\mathcal L_0.
$$

Its divergence is $(\Box\phi+m^2\phi)\partial^\nu\phi$, which vanishes on the [Klein-Gordon equation](../../../../../klein-gordon-equation.md). With vanishing flux at spatial infinity, the charges are conserved. In particular,

$$
\boxed{H_{\rm cl}=\frac12\int d^3x\,[\pi^2+|\nabla\phi|^2+m^2\phi^2],\qquad P^i_{\rm cl}=-\int d^3x\,\pi\,\partial_i\phi.}
$$

The minus sign is required because $P^i=\int T^{0i}$ and $\partial^i=-\partial_i$. These are the [four-momentum of a free real scalar field](../../../../../four-momentum-of-a-free-real-scalar-field.md).

For [canonical quantization](../../../../../canonical-quantization.md), impose $[\phi(\mathbf x),\pi(\mathbf y)]=i\delta^3(\mathbf x-\mathbf y)$, with both equal-time field-field commutators zero. Inverting the mode expansion gives

$$
a_{\mathbf p}=\int d^3x\,e^{-i\mathbf p\cdot\mathbf x}\left(\sqrt{E_{\mathbf p}/2}\,\phi(\mathbf x)+\frac{i\pi(\mathbf x)}{\sqrt{2E_{\mathbf p}}}\right).
$$

The equal-time [canonical commutation relation](../../../../../canonical-commutation-relation.md) then yields

$$
\boxed{[a_{\mathbf p},a_{\mathbf q}^\dagger]=(2\pi)^3\delta^3(\mathbf p-\mathbf q),\qquad[a_{\mathbf p},a_{\mathbf q}]=[a_{\mathbf p}^\dagger,a_{\mathbf q}^\dagger]=0.}
$$

For example, the two mixed field-momentum terms in the first commutator have coefficients $\frac12\sqrt{E_{\mathbf p}/E_{\mathbf q}}$ and $\frac12\sqrt{E_{\mathbf q}/E_{\mathbf p}}$; the delta function sets their sum to one.

Insert the mode expansion into the quadratic energy. Spatial integration supplies $(2\pi)^3\delta^3(\mathbf p\pm\mathbf q)$. In the $aa$ and $a^\dagger a^\dagger$ terms, the coefficient is proportional to $-E_{\mathbf p}^2+\mathbf p^2+m^2=0$. The remaining terms give

$$
H_{\rm bare}=\frac12\int\frac{d^3p}{(2\pi)^3}E_{\mathbf p}(a_{\mathbf p}a_{\mathbf p}^\dagger+a_{\mathbf p}^\dagger a_{\mathbf p})=\int\frac{d^3p}{(2\pi)^3}E_{\mathbf p}a_{\mathbf p}^\dagger a_{\mathbf p}+E_0.
$$

Here $E_0$ is the divergent [zero-point energy](../../../../../zero-point-energy.md), formally $\frac12\int d^3p\,E_{\mathbf p}\delta^3(0)$. Thus the vacuum-free energy formula requires [normal ordering](../../../../../normal-ordering.md), or equivalently subtraction of this constant. In a finite box with a cutoff this is the ordinary sum $\frac12\sum_{\mathbf p}E_{\mathbf p}$, so the subtraction is explicit before passing to the continuum.

Likewise, use the Hermitian momentum expression $-\frac12\int(\pi\nabla\phi+\nabla\phi\,\pi)d^3x$. Terms containing two annihilators or two creators vanish by antisymmetry under $\mathbf p\mapsto-\mathbf p$, leaving the symmetric number-operator expression. Its vacuum term is zero with an inversion-symmetric regulator. Therefore the [normal-ordered free scalar four-momentum](../../../../../normal-ordered-free-scalar-four-momentum.md) is

$$
\boxed{H=\int\frac{d^3p}{(2\pi)^3}E_{\mathbf p}a_{\mathbf p}^\dagger a_{\mathbf p},\qquad\mathbf P=\int\frac{d^3p}{(2\pi)^3}\mathbf p\,a_{\mathbf p}^\dagger a_{\mathbf p}.}
$$

The [creation operator](../../../../../creation-operator.md) commutators follow directly from $[a_{\mathbf q}^\dagger a_{\mathbf q},a_{\mathbf p}^\dagger]=a_{\mathbf q}^\dagger(2\pi)^3\delta^3(\mathbf q-\mathbf p)$:

$$
\boxed{[H,a_{\mathbf p}^\dagger]=E_{\mathbf p}a_{\mathbf p}^\dagger,\qquad[P^i,a_{\mathbf p}^\dagger]=p^i a_{\mathbf p}^\dagger.}
$$

Starting from a vacuum annihilated by every $a_{\mathbf p}$, each creation adds a particle of mass $m$, energy $E_{\mathbf p}$ and momentum $\mathbf p$. The [real scalar field](../../../../../real-scalar-field.md) has one spin-zero species: its antiparticle is the same species. Products of [creation operators](../../../../../creation-operator.md) commute, so multiparticle states are invariant under exchange of their labels. In a normalized discrete mode, $(a^\dagger)^r|0\rangle/\sqrt{r!}$ exists for every $r\ge0$; there is no exclusion restriction. These are [bosonic statistics from commuting creation operators](../../../../../bosonic-statistics-from-commuting-creation-operators.md) and prove [Bose-Einstein statistics](../../../../../bose-einstein-statistics.md). For completeness, the single-mode thermal sum $\sum_{r\ge0}e^{-\beta Er}$ gives $\langle r\rangle=(e^{\beta E}-1)^{-1}$, the [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md) at zero chemical potential.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
