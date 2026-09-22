<h1 id="33b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $u=kr-l\pi/2$. Since

$$
A_l\sin u-B_l\cos u
=\frac{-iA_l-B_l}{2}e^{iu}
+\frac{iA_l-B_l}{2}e^{-iu},
$$

the outgoing-to-incoming coefficient ratio is $-S_l$. Hence the [Partial-wave S-matrix](../../../../../../partial-wave-s-matrix.md) element and [scattering phase shift](../../../../../../scattering-phase-shift.md) are

$$
\boxed{
S_l(k)=\frac{A_l(k)-iB_l(k)}{A_l(k)+iB_l(k)}
=e^{2i\delta_l(k)},
\qquad
\tan\delta_l(k)=-\frac{B_l(k)}{A_l(k)}.}
$$

The [scattering length from a partial-wave S-matrix](../../../../../../scattering-length-from-a-partial-wave-s-matrix.md) is

$$
\boxed{
a_s=-\lim_{k\to0}\frac{\tan\delta_0(k)}k
=\lim_{k\to0}\frac{B_0(k)}{kA_0(k)}.}
$$

For the stated [S-wave scattering](../../../../../../s-wave-quantum-scattering.md) solution, $\tanh(\lambda r)\to1$ as $r\to\infty$, so

$$
\psi(r)\sim\frac{e^{-ikr}}r
+\frac{k+i\lambda}{k-i\lambda}\frac{e^{ikr}}r.
$$

Using the same incoming/outgoing convention,

$$
\boxed{
S_0(k)=-\frac{k+i\lambda}{k-i\lambda}
=\frac{\lambda-ik}{\lambda+ik}.}
$$

Therefore

$$
\boxed{
\delta_0(k)=-\tan^{-1}\frac{k}{\lambda}\pmod\pi,
\qquad
a_s=\frac1\lambda.}
$$

The [analytic continuation](../../../../../../analytic-continuation.md) of $S_0$ has a [bound-state pole of the scattering amplitude](../../../../../../bound-state-pole-of-the-scattering-amplitude.md) at $k=i\lambda$ in the upper half-plane. Since $E=\hbar^2k^2/(2m)$, this gives

$$
\boxed{E_{\rm bound}=-\frac{\hbar^2\lambda^2}{2m}.}
$$

To extract the bound-state wavefunction, multiply the scattering solution by $k-i\lambda$ and take the pole limit:

$$
\begin{aligned}
\psi_{\rm bound}(r)
&\propto i\lambda[1+\tanh(\lambda r)]e^{-\lambda r}/r\\
&\propto \frac{\operatorname{sech}(\lambda r)}r.
\end{aligned}
$$

Thus the unnormalized exterior solution is

$$
\boxed{\psi_{\rm bound}(r)\propto
\frac{\operatorname{sech}(\lambda r)}r,\qquad r>r_0.}
$$

These data are collected in the [Hyperbolic-tangent S-wave exterior solution](../../../../../../hyperbolic-tangent-s-wave-exterior-solution.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [33B](../../33b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
