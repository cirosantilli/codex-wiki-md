<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here the map direction is opposite to Question 2: write $\phi:U\to D$, with $\phi(0)=0$ and $\phi(1)=1$. The separation condition makes $U$ agree with $D$ near $1$. [Schwarz reflection](../../../../../../schwarz-reflection-principle.md) across that analytic boundary arc therefore defines the boundary derivative, whose modulus is positive.

For ordinary [Brownian motion](../../../../../../brownian-motion-split.md) $W$ started at $0$, let $\sigma_U$ be its first exit from $U$. Take sufficiently short arcs $I_\epsilon$ around $1$. They are also arcs of $\partial U$. The event that $W$ stays in $U$ until its disc exit and exits in $I_\epsilon$ is exactly the event $W_{\sigma_U}\in I_\epsilon$. Therefore the conditional avoidance probability is

$$
\frac{\omega_U(0,I_\epsilon)}{\omega_D(0,I_\epsilon)}.
$$

[Conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md) gives $\omega_U(0,I_\epsilon)=\omega_D(0,\phi(I_\epsilon))$. At the disc center [harmonic measure](../../../../../../harmonic-measure.md) is normalized arc length, so the ratio tends to $|\phi'(1)|$.

To justify that this limit is the avoidance probability for the point-conditioned diffusion, one may use the stopped transform directly. Its probability of reaching a smooth boundary arc at $1$ before any other boundary of $U$ is the mass at that pole in the transformed [harmonic measure](../../../../../../harmonic-measure.md). All other exit points have weights $h(w)$ and represent failure. Equivalently integrate the Poisson-kernel density at $1$ for $U$ and divide by that for $D$. This gives the boundary-density ratio above, without assuming that a full-path avoidance event is a continuity set for arbitrary weak convergence. The kernels transform by the boundary Jacobian:

$$
P_U(0,1)=P_D(\phi(0),\phi(1))\,|\phi'(1)|.
$$

Consequently

$$
\boxed{\mathbb P(B[0,\tau)\subset U)=\frac{P_U(0,1)}{P_D(0,1)}=|\Phi_U'(1)|.}
$$

There is no extra factor of $|\Phi_U'(0)|$. The starting point is fixed and the conditioning concerns boundary harmonic-measure density. In this normalization the boundary derivative is a positive real, so it may also be written $\Phi_U'(1)$. It is at most one by the probability interpretation. Given avoidance, the mapped path is the same conditioned [Brownian motion](../../../../../../brownian-motion-split.md) up to conformal time change; this is [radial restriction for a conditioned Brownian path](../../../../../../radial-restriction-for-a-conditioned-brownian-path.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
