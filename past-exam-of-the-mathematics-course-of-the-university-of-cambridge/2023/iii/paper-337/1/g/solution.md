<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [analytic continuation](../../../../../../analytic-continuation.md) from bosonic imaginary frequency to a retarded frequency is $i\omega_n\mapsto\omega+i0^+$. Thus

$$
\boxed{
G_R(\omega,\mathbf k)
=\frac{vg}{N}
\frac1{v^2k^2+m(T)^2-(\omega+i0^+)^2}.}
$$

Writing $E_k=\sqrt{v^2k^2+m(T)^2}$ and using the [Sokhotski–Plemelj formula](../../../../../../sokhotski-plemelj-theorem.md) gives, in this sign convention,

$$
\boxed{
\operatorname{Im}G_R(\omega,\mathbf k)
=\frac{\pi vg}{2NE_k}
\left[\delta(\omega-E_k)-\delta(\omega+E_k)\right].}
$$

The opposite overall convention for the [retarded Green function](../../../../../../retarded-green-function.md) reverses this sign; the corresponding [spectral function](../../../../../../spectral-function.md) is conventionally chosen positive at positive frequency.

Near the [quantum critical point](../../../../../../quantum-critical-point.md), $m/T$ is a function only of $\Delta/T$. The Green function has the scaling form

$$
G_R(\omega,k;T,\Delta)
=\frac{vg}{N}T^{-2}
\mathcal G\left(\frac\omega T,
\frac{vk}{T},\frac\Delta T\right),
$$

with

$$
\mathcal G^{-1}
=\left(\frac{vk}{T}\right)^2
+\left[2\operatorname{arsinh}
\left(\frac12e^{\Delta/(2T)}\right)\right]^2
-\left(\frac{\omega+i0^+}{T}\right)^2.
$$

This is [quantum critical scaling](../../../../../../quantum-critical-scaling.md) with dynamical critical exponent $z=1$ and leading large-$N$ anomalous dimension $\eta=0$.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
