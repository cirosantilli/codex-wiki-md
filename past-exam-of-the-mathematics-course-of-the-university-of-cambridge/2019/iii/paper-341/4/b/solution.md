<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [Fourier mode](../../../../../../fourier-mode.md), the amplification polynomial is

$$
\xi^2-(1-2\mu)(1-e^{i\theta})\xi-e^{i\theta}=0.
$$

Put $a=1-2\mu$ and $\xi=e^{i\theta/2}\eta$. The roots become

$$
\eta_\pm=-ia\sin(\theta/2)\pm\sqrt{1-a^2\sin^2(\theta/2)}.
$$

If $|a|<1$, the square root is real, both roots have [modulus](../../../../../../modulus.md) one, and their separation is at least $2\sqrt{1-a^2}>0$. The companion [matrix](../../../../../../matrix.md) has [eigenvectors](../../../../../../eigenvector.md) $(\xi_\pm,1)^T$, so their uniform separation gives a mesh-independent bound on its powers. By [power boundedness of a two-level Fourier scheme](../../../../../../power-boundedness-of-a-two-level-fourier-scheme.md) and the discrete [Fourier transform](../../../../../../fourier-transform.md), this proves stability for $0<\mu<1$.

If $|a|>1$, choose $\theta=\pi$. The roots have product of [modulus](../../../../../../modulus.md) one and unequal [moduli](../../../../../../modulus.md), so one has [modulus](../../../../../../modulus.md) greater than one. The scheme is unstable.

The boundary cases require more than a root-modulus check. At $\theta=\pi$, $\mu=0$ gives $(\xi-1)^2=0$, while $\mu=1$ gives $(\xi+1)^2=0$. The companion [matrices](../../../../../../matrix.md) have nontrivial [Jordan blocks](../../../../../../jordan-block.md) and solutions of the form $(A+Bn)(\pm1)^n$. Their linear growth rules out a uniform stability bound. This mode occurs on even periodic grids, which are enough to disprove mesh-uniform stability at the endpoints.

Therefore the stable range is exactly

$$
\boxed{0<\mu<1.}
$$

Within this range, second-order convergence additionally requires two appropriately accurate starting time levels. The unit-modulus parasitic root near $\theta=0$ does not decay, so poor initialization cannot be repaired by the scheme.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
