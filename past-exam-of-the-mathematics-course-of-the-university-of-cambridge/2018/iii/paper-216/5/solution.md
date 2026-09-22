<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $\phi_d(z)=(2\pi)^{-d/2}\exp(-\|z\|^2/2)$ be the standard [multivariate normal density](../../../../../multivariate-normal-density.md). Independence gives the [proposal distribution](../../../../../proposal-distribution.md) density

$$
q(x,y)=\int\phi_d(y-Ax)\,\nu(dA).
$$

For an [orthogonal matrix](../../../../../orthogonal-matrix.md) $A$,

$$
\|y-Ax\|=\|A^Ty-x\|=\|x-A^Ty\|.
$$

The isotropic Gaussian density is unchanged by this transformation. Since $A^T$ has the same distribution as $A$,

$$
q(x,y)=\int\phi_d(x-A^Ty)\,\nu(dA)=\int\phi_d(x-Ay)\,\nu(dA)=q(y,x).
$$

Thus this is an [orthogonal-mixture Metropolis proposal](../../../../../orthogonal-mixture-metropolis-proposal.md) with a symmetric density; inversion invariance, rather than any assumption of a uniform distribution on orthogonal matrices, is what is needed.

With $\alpha(x,y)=\min\{1,\pi(y)/\pi(x)\}$, the accepted off-diagonal transitions satisfy

$$
\pi(x)q(x,y)\alpha(x,y)=q(x,y)\min\{\pi(x),\pi(y)\}
=\pi(y)q(y,x)\alpha(y,x).
$$

The rejection part is supported on the diagonal and satisfies [detailed balance](../../../../../detailed-balance.md) automatically. Values of the acceptance rule at starting points where $\pi(x)=0$ can be specified separately; they do not affect stationarity under $\pi$. Therefore the [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) kernel is reversible with invariant density $\pi$, proving

$$
\boxed{\pi\text{ is a stationary distribution}.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 216](../../paper-216-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
