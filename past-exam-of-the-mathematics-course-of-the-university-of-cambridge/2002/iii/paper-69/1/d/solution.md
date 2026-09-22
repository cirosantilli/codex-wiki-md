<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume the pinning coefficient $t>0$. Here $t$ belongs to an actual energy, so its Boltzmann coefficient is $\beta t$. The quadratic kernel and [covariance](../../../../../../covariance.md) become

$$
H_2+V=\frac12\int_{\mathbf q}(\sigma q^2+t)|h_{\mathbf q}|^2,\qquad
\langle h_{\mathbf q}h_{\mathbf q'}\rangle=\frac{k_BT}{\sigma q^2+t}(2\pi)^D\delta^{(D)}(\mathbf q+\mathbf q').
$$

Therefore the [pinned capillary-wave correlation](../../../../../../pinned-capillary-wave-correlation.md) is

$$
\boxed{B_t(r)=\frac{2k_BT}{\sigma}\int_{\mathbf q}\frac{1-\cos(\mathbf q\cdot\mathbf r)}{q^2+\xi^{-2}},\qquad \xi=\sqrt{\sigma/t}.}
$$

The normal-translation [symmetry](../../../../../../symmetry-physics.md) is now explicitly broken, and the formerly massless [Goldstone mode](../../../../../../goldstone-boson.md) has a restoring term. For $r\ll\xi$, but beyond the microscopic cutoff, the unpinned behavior is recovered. For $r\gg\xi$, the connected height [covariance](../../../../../../covariance.md) decays and $B_t$ approaches $2\langle h^2\rangle$, so roughness no longer grows without bound even for $d=2,3$.

In internal dimension one the exact continuum answer is

$$
B_t(r)=\frac{k_BT\xi}{\sigma}(1-e^{-|r|/\xi}).
$$

In internal dimension two the connected [covariance](../../../../../../covariance.md) at $r>0$ is $k_BT K_0(r/\xi)/(2\pi\sigma)$, where $K_0$ is a [modified Bessel function](../../../../../../modified-bessel-function.md); its zero-separation value needs the cutoff and the saturation value grows as $(k_BT/\pi\sigma)\log(\xi/a)$ for $\xi\gg a$. In internal dimension three the connected [covariance](../../../../../../covariance.md) is approximately $k_BT e^{-r/\xi}/(4\pi\sigma r)$ beyond the cutoff. Thus pinning replaces the long-distance massless tails by exponential decay. A negative $t$ would destabilize the quadratic [statistical Hamiltonian](../../../../../../statistical-hamiltonian.md) rather than bind the membrane.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
