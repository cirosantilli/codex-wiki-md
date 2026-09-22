<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any fixed subregion $\Omega$, with no internal [heat](../../../../../../heat-split.md) generation, [conservation of energy](../../../../../../conservation-of-energy.md) says that the rate of stored thermal [energy](../../../../../../energy-split.md) equals the incoming [heat flux](../../../../../../heat-flux-density.md):

$$
\frac{d}{dt}\iiint_\Omega\rho cT\,dV=-\iint_{\partial\Omega}\mathbf q\cdot\mathbf n\,dA.
$$

The minus sign is needed because $\mathbf q\cdot\mathbf n>0$ denotes outgoing [heat flux](../../../../../../heat-flux-density.md). Substitute [Fourier's law](../../../../../../fourier-s-law.md) $\mathbf q=-k\nabla T$ and apply the [divergence theorem](../../../../../../divergence-theorem.md):

$$
\iiint_\Omega\rho cT_t\,dV
=\iint_{\partial\Omega}k\nabla T\cdot\mathbf n\,dA
=\iiint_\Omega\nabla\cdot(k\nabla T)\,dV.
$$

Here differentiation under the [integral](../../../../../../integral-split.md) uses a fixed region and sufficient regularity of $T$. Since the identity holds for every $\Omega$, continuity of the integrands gives the local [heat equation](../../../../../../heat-equation.md)

$$
\boxed{\rho cT_t=\nabla\cdot\bigl(k(\mathbf x)\nabla T\bigr).}
$$

For spatially varying [thermal conductivity](../../../../../../thermal-conductivity.md), the [product rule](../../../../../../product-rule.md) gives $\nabla\cdot(k\nabla T)=k\nabla^2T+\nabla k\cdot\nabla T$; the second term cannot generally be discarded.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
