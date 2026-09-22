<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A free nonrelativistic [Gaussian wave packet](../../../../../../gaussian-wave-packet.md) with initial position variance $\sigma_0^2$ has [wave function](../../../../../../wave-function.md)

$$
\psi(x,0)=(2\pi\sigma_0^2)^{-1/4}e^{-x^2/(4\sigma_0^2)}.
$$

The free dispersion relation $E=p^2/(2m)$ makes its different [momentum](../../../../../../momentum.md) components acquire different phases. Fourier evolution gives a position variance

$$
\boxed{\sigma(t)^2=\sigma_0^2\left[1+\left(\frac{\hbar t}{2m\sigma_0^2}\right)^2\right].}
$$

This spreading is ordinary unitary dynamics. A Gaussian already has nonzero tails initially, so its width increase alone is not an example of information suddenly appearing outside an initially compact support.

For genuinely compactly supported nonzero initial data, the nonrelativistic free kernel yields

$$
\psi(x,t)=\sqrt{\frac{m}{2\pi i\hbar t}}e^{imx^2/(2\hbar t)}\int e^{-imxy/(\hbar t)}e^{imy^2/(2\hbar t)}\psi(y,0)\,dy.
$$

At $t\ne0$, the integral is an entire Fourier transform of a compactly supported function. It cannot vanish on an open exterior interval unless the whole transform, and hence the initial state, vanishes. Thus this theory has no strict finite propagation cone for nonzero compact initial [wave functions](../../../../../../wave-function.md). It is a nonrelativistic theory, so that result is not a contradiction in a fundamental relativistic field theory.

Positive-energy relativistic particle descriptions raise a subtler issue. The [Hegerfeldt theorem](../../../../../../hegerfeldt-theorem.md) concerns a Hamiltonian bounded below and a positive localization effect $A$. The function $p_A(t)=\|A^{1/2}e^{-iHt}\psi\|^2$ either vanishes identically or is nonzero for almost every time. Vanishing for an open interval makes the analytic continuation of the vector matrix elements vanish identically. A sharp exterior localization probability which remains zero for a nonzero time interval but becomes positive later is therefore incompatible with those assumptions.

The conclusion restricts simultaneous assumptions about positive energy and sharp particle localization. It does not establish an admissible procedure for controllable superluminal messaging. A particle-position projection need not belong to the algebra of a physically local relativistic measurement, and strictly localized one-particle preparation can fail the required assumptions. In field theory the appropriate locality test concerns [local operations](../../../../../../local-quantum-operation.md) and [observables](../../../../../../observable.md), not merely pointwise values of a one-particle [wave function](../../../../../../wave-function.md). **Localization, propagation of field disturbances and transmission of information must be distinguished.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
