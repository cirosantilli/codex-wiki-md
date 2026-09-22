<h1 id="16d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the [Fourier transform](../../../../../../fourier-transform.md) in $x$. The transform of the source is $\delta(t-t')e^{-ikx'}$, so the [Green function](../../../../../../green-s-function.md) equation becomes

$$
\partial_t\widetilde G+Dk^2\widetilde G=\delta(t-t')e^{-ikx'}.
$$

Choose the [causal Green function](../../../../../../causal-green-function.md), zero for $t<t'$. Away from $t'$ the solution is a decaying exponential, and integrating across $t'$ gives the jump $\widetilde G(t'+)-\widetilde G(t'-)=e^{-ikx'}$. Therefore

$$
\boxed{\widetilde G=H(t-t')e^{-ikx'}e^{-Dk^2(t-t')}.}
$$

The phase shifts the kernel's centre to $x'$. Applying the inverse [Fourier transform](../../../../../../fourier-transform.md) and the [Fourier transform of a Gaussian](../../../../../../fourier-transform-of-a-gaussian.md) with $a=D(t-t')$ gives

$$
\boxed{G=\frac{H(t-t')}{\sqrt{4\pi D(t-t')}}\exp\left[-\frac{(x-x')^2}{4D(t-t')}\right].}
$$

For positive elapsed time this [heat kernel](../../../../../../heat-kernel.md) solves the homogeneous diffusion equation and has unit integral; as elapsed time tends to zero it approaches the spatial delta distribution, supplying the required impulse.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16D](../../16d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
