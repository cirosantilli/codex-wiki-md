<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A weight-$k$ [modular form](../../../../../modular-form.md) for $\Gamma=SL_2(\mathbb Z)$ is a [holomorphic function](../../../../../holomorphic-function.md) $f$ on the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) satisfying

$$
f\left(\frac{a\tau+b}{c\tau+d}\right)=(c\tau+d)^kf(\tau)
\qquad\left(\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma\right),
$$

and [holomorphic at a cusp](../../../../../holomorphic-at-a-cusp.md). Since the full [modular group](../../../../../modular-group.md) has one cusp class, this last condition means that the period-one function has a convergent expansion $f(\tau)=\sum_{n\geq0}a_nq^n$, $q=e^{2\pi i\tau}$, near infinity. A [cusp form](../../../../../cusp-form.md) has $a_0=0$. The element $-I$ makes a nonzero weight odd form impossible.

For weight zero, $f$ descends to a [holomorphic function](../../../../../holomorphic-function.md) on the quotient of the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) by the [modular group](../../../../../modular-group.md). At an elliptic fixed point, invariance under its finite stabilizer makes the local Taylor series a series in the quotient coordinate. At the cusp, the $q$ expansion extends it over $q=0$. The [standard fundamental domain of the modular group](../../../../../standard-fundamental-domain-of-the-modular-group.md), with its boundary identified and its cusp added, is a compact [Riemann surface](../../../../../riemann-surfaces.md), the [compactified modular curve](../../../../../compactified-modular-curve.md) $X(1)$. The [maximum modulus principle](../../../../../maximum-modulus-principle.md) now proves

$$
\boxed{M_0(SL_2(\mathbb Z))=\mathbb C.}
$$

Holomorphy at the cusp is essential to this conclusion.

<a id="2/image-the-standard-modular-fundamental-domain-with-paired-vertical-boundaries-paired-circular-arcs-and-the-added-cusp-at-infinity"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126-modular-domain.png)

**[Figure 1](#2/image-the-standard-modular-fundamental-domain-with-paired-vertical-boundaries-paired-circular-arcs-and-the-added-cusp-at-infinity). The standard modular fundamental domain with paired vertical boundaries, paired circular arcs, and the added cusp at infinity**.

For positive even $k\geq4$, define the unnormalized [Eisenstein series](../../../../../eisenstein-series.md)

$$
G_k(\tau)=\sum_{(m,n)\in\mathbb Z^2\setminus\{(0,0)\}}(m\tau+n)^{-k}.
$$

The real-linear map $(m,n)\mapsto m\tau+n$ is invertible, and on a compact subset of the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) its norm is uniformly comparable to $\sqrt{m^2+n^2}$. Thus the sum converges absolutely and locally uniformly for $k>2$, proving [holomorphy](../../../../../holomorphic-function.md). For $\gamma=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$,

$$
m\gamma\tau+n=\frac{(ma+nc)\tau+(mb+nd)}{c\tau+d}.
$$

The map $(m,n)\mapsto(ma+nc,mb+nd)$ is a bijection on the nonzero integer pairs, giving $G_k(\gamma\tau)=(c\tau+d)^kG_k(\tau)$.

For the expansion, the [cotangent partial-fraction Fourier kernel](../../../../../cotangent-partial-fraction-fourier-kernel.md) follows by differentiating the partial-fraction expansion of $\pi\cot\pi z$ and its geometric-series expansion $-\pi i(1+2\sum_{r\geq1}e^{2\pi i rz})$, valid for $\operatorname{Im}z>0$. It gives, for even $k\geq2$,

$$
\sum_{n\in\mathbb Z}(z+n)^{-k}
=\frac{(2\pi i)^k}{(k-1)!}\sum_{r\geq1}r^{k-1}e^{2\pi i rz}.
$$

The $m=0$ part of $G_k$ is $2\zeta(k)$, where $\zeta$ is the [Riemann zeta function](../../../../../riemann-zeta-function.md); positive and negative $m$ contribute equally. Apply the kernel at $z=m\tau$ for $m>0$, and regroup the absolutely convergent sum according to $N=mr$. With the [divisor sum](../../../../../divisor-sum.md) $\sigma_{k-1}(N)=\sum_{r\mid N}r^{k-1}$, this proves

$$
\boxed{G_k(\tau)=2\zeta(k)+\frac{2(2\pi i)^k}{(k-1)!}\sum_{N\geq1}\sigma_{k-1}(N)q^N.}
$$

The expansion has no negative powers and converges for $|q|<1$, so it also proves [holomorphy at a cusp](../../../../../holomorphic-at-a-cusp.md) and completes the proof of modularity.

The supplied zeta values yield the [Fourier expansion of a normalized Eisenstein series](../../../../../fourier-expansion-of-a-normalized-eisenstein-series.md)

$$
E_4=1+240S_3,\qquad E_6=1-504S_5,\qquad
S_j=\sum_{n\geq1}\sigma_j(n)q^n.
$$

Both $E_4^3$ and $E_6^2$ are [modular forms](../../../../../modular-form.md) of weight twelve. Their constant terms cancel, so their difference divided by $1728$ is a [cusp form](../../../../../cusp-form.md). Integrality requires an argument: dividing an integral series by $1728$ alone would not suffice. Expanding directly gives the [integrality identity for the modular discriminant](../../../../../integrality-identity-for-the-modular-discriminant.md)

$$
\Delta=\frac{5S_3+7S_5}{12}+100S_3^2+8000S_3^3-147S_5^2.
$$

For every integer $d$, $5d^3+7d^5$ is divisible by twelve. Modulo three, $d^3\equiv d^5\equiv d$; modulo four, an even $d$ makes both powers divisible by four, while an odd $d$ has $d^3\equiv d^5\equiv d\pmod4$. Thus each coefficient $(5\sigma_3(n)+7\sigma_5(n))/12$ is integral. The other three series visibly have integral coefficients, proving

$$
\boxed{\Delta\in S_{12}(SL_2(\mathbb Z)),\qquad\Delta\in q\mathbb Z[[q]],\qquad a_1(\Delta)=1.}
$$

This proves integrality without assuming a product expansion for the [modular discriminant](../../../../../modular-discriminant.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 126](../../paper-126-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
