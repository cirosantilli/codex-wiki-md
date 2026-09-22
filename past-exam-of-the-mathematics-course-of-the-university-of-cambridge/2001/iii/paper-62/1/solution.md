<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [canonical quantization](../../../../../canonical-quantization.md) with $[\hat q,\hat p]=i\hbar$, $\hat p=-i\hbar\partial_q$, and $\hat H=\hat p^2/(2m)+V(\hat q)$. Assume a real [potential energy](../../../../../potential-energy.md) with the regularity and lower-bound conditions needed for a self-adjoint [Hamiltonian](../../../../../hamiltonian.md) and its [Trotter product formula](../../../../../lie-product-formula.md); singular potentials require their domain and limiting prescription to be specified separately. The transition amplitude is $K(\beta,\alpha;T)=\langle\beta|e^{-iT\hat H/\hbar}|\alpha\rangle$.

Take $\delta=T/N$, $q_0=\alpha$, $q_N=\beta$, and choose the left-endpoint [potential energy](../../../../../potential-energy.md) convention. The precise time-sliced [phase-space path integral](../../../../../phase-space-path-integral.md) is

$$
K_N=\int\prod_{j=1}^{N-1}dq_j\prod_{j=1}^{N}\frac{dp_j}{2\pi\hbar}
\exp\left\{\frac{i}{\hbar}\sum_{j=1}^{N}\left[p_j(q_j-q_{j-1})-\delta\left(\frac{p_j^2}{2m}+V(q_{j-1})\right)\right]\right\}.
$$

The endpoint positions are fixed and the momenta are unconstrained. Its continuum notation is

$$
\boxed{K=\int_{q(0)=\alpha}^{q(T)=\beta}\mathcal Dq\,\mathcal Dp\;
\exp\left[\frac{i}{\hbar}\int_0^T(p\dot q-H(p,q))dt\right],}
$$

where the functional measure means the displayed limit, not an unspecified product of unnormalized measures.

At each slice, complete the square in [momentum](../../../../../momentum.md). With the square-root branch selected by continuation from positive Euclidean time,

$$
\int\frac{dp}{2\pi\hbar}\exp\left[\frac{i}{\hbar}\left(p\Delta q-\frac{\delta p^2}{2m}\right)\right]
=\left(\frac{m}{2\pi i\hbar\delta}\right)^{1/2}
\exp\left[\frac{im(\Delta q)^2}{2\hbar\delta}\right].
$$

Thus the [time-sliced equivalence of phase-space and configuration-space path integrals](../../../../../time-sliced-equivalence-of-phase-space-and-configuration-space-path-integrals.md) holds already at finite $N$:

$$
K_N=\left(\frac{m}{2\pi i\hbar\delta}\right)^{N/2}
\int\prod_{j=1}^{N-1}dq_j\;
\exp\left\{\frac{i}{\hbar}\sum_{j=1}^{N}\left[\frac{m(q_j-q_{j-1})^2}{2\delta}-\delta V(q_{j-1})\right]\right\}.
$$

This defines the [configuration-space path integral](../../../../../configuration-space-path-integral.md)

$$
\boxed{K=\int_{q(0)=\alpha}^{q(T)=\beta}\mathcal Dq\;
\exp\left[\frac{i}{\hbar}\int_0^T\left(\frac m2\dot q^2-V(q)\right)dt\right].}
$$

There are $N$ Gaussian prefactors but only $N-1$ coordinate integrations. Omitting that distinction would change the kernel normalization. The paths integrated in the limit need not be differentiable; the kinetic action notation stands for the lattice difference expression.

To identify this with the operator amplitude, normalize $\langle q|p\rangle=(2\pi\hbar)^{-1/2}e^{ipq/\hbar}$. The kernel of one product factor is exactly

$$
\langle q_j|e^{-i\delta\hat p^2/(2m\hbar)}e^{-i\delta V(\hat q)/\hbar}|q_{j-1}\rangle
=\int\frac{dp_j}{2\pi\hbar}\;e^{ip_j(q_j-q_{j-1})/\hbar-i\delta p_j^2/(2m\hbar)-i\delta V(q_{j-1})/\hbar}.
$$

Insert $N-1$ position resolutions of the identity between factors. Their product is precisely $K_N$. The [Trotter product formula](../../../../../lie-product-formula.md) then gives

$$
\left(e^{-iT\hat p^2/(2mN\hbar)}e^{-iTV(\hat q)/(N\hbar)}\right)^N\longrightarrow e^{-iT\hat H/\hbar},
$$

so both functional integrals represent the same canonical kernel. One can define the finite integrals first at $T=-i\tau$, $\tau>0$, where the Gaussian [momentum](../../../../../momentum.md) and coordinate kernels converge, and then continue to the real-time boundary value. Alternatively use an equivalent oscillatory damping prescription. Operator convergence fixes the distributional kernel limit; it need not imply pointwise convergence at every endpoint for every admissible [potential energy](../../../../../potential-energy.md). There is no operator-ordering ambiguity for this separated kinetic-plus-potential [Hamiltonian](../../../../../hamiltonian.md) once the common slicing convention is fixed.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
