<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) for the spatial [Cauchy problem](../../../../../../cauchy-problem.md), or its periodic analogue, and regard the two starting levels as independently perturbed data. A [Fourier mode](../../../../../../fourier-mode.md) with spatial factor $e^{im\theta}$ has amplification roots $G$ satisfying

$$
G^2-(2\mu-1)(e^{i\theta}-1)G-e^{i\theta}=0.
$$

Put $c=2\mu-1$ and $G=e^{i\theta/2}q$. Then

$$
q^2-2ic\sin(\theta/2)q-1=0,\qquad
q_\pm=ic\sin(\theta/2)\pm
\sqrt{1-c^2\sin^2(\theta/2)}.
$$

If $|c|<1$, both roots have modulus one and their separation is bounded below uniformly in frequency:

$$
|G_+-G_-|\geq2\sqrt{1-c^2}>0.
$$

The [uniform power bound from separated amplification roots](../../../../../../uniform-power-bound-from-separated-amplification-roots.md) now controls the two-level companion [matrix](../../../../../../matrix.md) for every time step. Its entries are uniformly bounded, and its eigenvector conditioning is bounded by the reciprocal root gap. The [Parseval identity](../../../../../../parseval-identity.md) transfers this frequency-uniform bound to the spatial $\ell^2$ norm. This proves stability, rather than merely checking each root's modulus.

If $|c|>1$, the frequency $\theta=\pi$ has a root outside the unit disk, so there is exponential instability. If $|c|=1$, the two roots at $\theta=\pi$ coincide on the unit circle. The companion [matrix](../../../../../../matrix.md) is not a scalar [matrix](../../../../../../matrix.md) and has a nontrivial [Jordan block](../../../../../../jordan-block.md); its powers grow linearly in the number of steps. Frequencies arbitrarily near that value produce the same lack of a uniform bound for localized Fourier packets, so this also invalidates Cauchy $\ell^2$ stability, not only periodic plane-wave stability. At $\mu=1$ the double amplification root is $-1$, and at $\mu=0$ it is $1$.

Therefore the full two-level stability range for a fixed positive Courant ratio is

$$
\boxed{0<\mu<1.}
$$

The endpoint $\mu=0$ is moreover not a positive time step. Bounds deteriorate as $\mu$ approaches either endpoint; the displayed range is not a uniform claim over ratios arbitrarily close to one. A prescribed starter that removes one special parasitic component can change behavior for selected initial data, but does not establish the requested unrestricted two-level stability.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
